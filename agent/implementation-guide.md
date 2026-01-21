# Implementation Guide

## For AI Platform Developers

This guide explains how to implement the Business Idea Validation Agent on various AI platforms (Claude, GPT, custom platforms, etc.)

## Architecture Overview

```
User Input
    ↓
System Prompt + Behavior Guidelines
    ↓
Skill Progression (1→2→3→4→5→6→7→8→9)
    ↓
Output Generation
    ↓
Markdown File → User Download
```

## Implementation Steps

### 1. Load System Prompt

**Primary file**: `/agent/system-prompt.md`

This contains:
- Agent role and mission
- Methodology overview
- Operating principles
- Core behavior rules

**Load this as**: System message / initial context

### 2. Load Behavior Guidelines

**Primary file**: `/agent/behavior-guidelines.md`

This contains:
- Detailed communication style rules
- Question patterns
- Response patterns
- Quality standards

**Load this as**: Additional system context or reference document

### 3. Initialize Conversation State

```javascript
{
  current_skill: 1,
  skills_completed: [],
  collected_data: {
    problem: null,
    customer_segments: null,
    value_proposition: null,
    solution: null,
    market: null,
    business_model: null,
    metrics: null,
    risks: null
  },
  user_preferences: {
    framework: 'lean_canvas', // or 'opportunity_assessment'
    detail_level: 'standard'   // or 'deep_dive'
  }
}
```

### 4. Skill Loading System

Each skill file (`/agent/skills/*.md`) contains:
- Purpose
- Questions to ask
- Information to collect
- Validation criteria
- Behavior guidelines for that skill

**Implementation approach**:

#### Option A: Load all skills at start
- Include all 9 skill files in context
- Agent references current skill based on state

#### Option B: Load skills dynamically
- Load only current skill into context
- Load next skill when transitioning
- Reduces context size

#### Option C: Embed in system prompt
- Consolidate all skills into single prompt
- Larger initial prompt, simpler state management

**Recommended**: Option A for simplicity, Option B for efficiency

### 5. Conversation Loop

```python
while current_skill <= 9:
    # Get user input
    user_message = get_user_input()

    # Load current skill context
    skill_context = load_skill(current_skill)

    # Generate response
    response = agent.respond(
        system_prompt=system_prompt,
        behavior_guidelines=behavior_guidelines,
        skill_context=skill_context,
        conversation_history=history,
        state=state,
        user_message=user_message
    )

    # Check if skill is complete
    if skill_is_complete(response, skill_context):
        collected_data[skill_name] = extract_data(conversation)
        current_skill += 1

    # Show response to user
    display(response)

    # If all skills complete, generate output
    if current_skill == 10:  # After skill 9
        generate_canvas(collected_data)
        break
```

### 6. Output Generation

**When**: After skill 9 completes and user confirms

**Process**:
1. Load template: `/templates/lean-canvas-template.md`
2. Fill template with `collected_data`
3. Mark unknowns as "TBD - Requires validation"
4. Generate filename: `[sanitized-idea-name]-validation-canvas.md`
5. Save to: `/outputs/[filename]`
6. Return download link to user

**Example**:
```python
def generate_canvas(collected_data):
    template = load_file('/templates/lean-canvas-template.md')

    # Replace placeholders
    output = template.replace('[IDEA NAME]', collected_data['idea_name'])
    output = output.replace('[Problem 1]', collected_data['problem']['pain_1'])
    # ... etc

    # Mark unknowns
    if not collected_data['unfair_advantage']:
        output = output.replace('[unfair advantage section]',
                               'TBD - Requires validation')

    # Generate filename
    filename = sanitize(collected_data['idea_name']) + '-validation-canvas.md'

    # Save
    save_file(f'/outputs/{filename}', output)

    return filename
```

## Platform-Specific Implementations

### Claude (via API or Claude Code)

```python
import anthropic

client = anthropic.Anthropic()

# Load system prompt
system_prompt = load_file('/agent/system-prompt.md')
behavior_guidelines = load_file('/agent/behavior-guidelines.md')
current_skill = load_file(f'/agent/skills/01-problem-definition.md')

messages = []

while True:
    response = client.messages.create(
        model="claude-3-5-sonnet-20241022",
        max_tokens=1024,
        system=f"{system_prompt}\n\n{behavior_guidelines}\n\n{current_skill}",
        messages=messages
    )

    # Handle response, update state, etc.
```

### GPT (via OpenAI API)

```python
from openai import OpenAI

client = OpenAI()

messages = [
    {"role": "system", "content": system_prompt + "\n" + behavior_guidelines}
]

response = client.chat.completions.create(
    model="gpt-4",
    messages=messages
)
```

### Custom Platform

Key requirements:
- Support for system prompts (agent instructions)
- Conversation history/context
- File generation capability
- State persistence between turns

## Advanced Features

### Multi-Session Support

Allow users to pause and resume:

```javascript
{
  session_id: 'uuid',
  created_at: timestamp,
  last_updated: timestamp,
  current_skill: 3,
  collected_data: {...},
  conversation_history: [...]
}
```

Save state to database/file after each turn.
Load state when user returns.

### Skill Skipping

Allow users to jump to specific skill:

```
User: "I want to work on pricing"
Agent: "Jumping to Business Model skill. What's your revenue model?"
```

Implementation:
- Map user intent to skill number
- Update `current_skill` state
- Load corresponding skill file

### Framework Switching

Support both Lean Canvas and Opportunity Assessment:

```python
if user_preferences['framework'] == 'opportunity_assessment':
    template = load_file('/templates/opportunity-assessment-template.md')
    skills = load_opportunity_skills()
else:
    template = load_file('/templates/lean-canvas-template.md')
    skills = load_lean_canvas_skills()
```

### Export Formats

**Markdown** (default):
```python
save_as_markdown(output, filename)
```

**PDF** (requires conversion):
```python
import markdown2
import pdfkit

html = markdown2.markdown(output)
pdfkit.from_string(html, f'{filename}.pdf')
```

**PNG/SVG** (visual canvas):
```python
# Use canvas rendering library
render_canvas_visual(collected_data, format='png')
```

## Testing

### Unit Tests

Test individual skill validation:

```python
def test_problem_definition_skill():
    skill = ProblemDefinitionSkill()

    # Test vague input
    response = skill.validate("People waste time")
    assert response.is_specific == False
    assert "more specific" in response.feedback

    # Test specific input
    response = skill.validate("Dev teams can't track dependencies")
    assert response.is_specific == True
```

### Integration Tests

Test full conversation flow:

```python
def test_full_validation_flow():
    agent = ValidationAgent()

    # Simulate complete conversation
    conversation = [
        ("What problem?", "Dev teams can't track dependencies"),
        ("Who experiences this?", "Engineering managers at 50-200 person SaaS companies"),
        # ... etc
    ]

    for question, answer in conversation:
        response = agent.process(answer)

    # Check output generated
    assert os.path.exists(f'/outputs/{agent.output_filename}')
```

### User Acceptance Tests

Test with real users:
- Clarity of questions
- Usefulness of challenges
- Quality of output
- Time to completion

## Deployment

### As Web App

```python
from flask import Flask, request, jsonify

app = Flask(__name__)

@app.route('/validate', methods=['POST'])
def validate():
    user_message = request.json['message']
    session_id = request.json['session_id']

    # Load session state
    state = load_session(session_id)

    # Process message
    response = agent.process(user_message, state)

    # Save state
    save_session(session_id, state)

    return jsonify({'response': response})
```

### As Chat Widget

Embed in existing products:

```html
<script src="validation-agent.js"></script>
<div id="validation-agent"></div>
<script>
  ValidationAgent.init({
    container: '#validation-agent',
    apiKey: 'your-key',
    onComplete: (canvas) => {
      console.log('Validation complete:', canvas)
    }
  })
</script>
```

### As CLI Tool

```bash
$ idea-validate

Let's validate your business idea. What problem does it solve?
> Dev teams can't track dependencies

✓ Got it. Who experiences this problem?
> Engineering managers

...
```

## Monitoring & Analytics

Track key metrics:

```python
{
  'sessions_started': 1000,
  'sessions_completed': 650,
  'completion_rate': 0.65,
  'avg_time_to_complete': '18 minutes',
  'avg_questions_per_skill': 2.3,
  'most_challenging_skill': 'Value Proposition',
  'user_satisfaction': 4.2
}
```

## Optimization

### Context Window Management

For large conversations:
- Summarize earlier skills once complete
- Keep only current skill details in full
- Archive completed skills to retrieval system

### Response Time

- Pre-load templates
- Cache skill files
- Use streaming responses for better UX

### Cost Optimization

- Use smaller models for simple validation checks
- Use larger models for complex challenges/synthesis
- Implement skill-specific model selection

## Troubleshooting

### Agent is too verbose
→ Strengthen brevity rules in system prompt
→ Add token limits per response

### Agent hallucinates data
→ Add explicit "no hallucination" rules
→ Require evidence for all claims

### Users get stuck
→ Add skill skip/resume functionality
→ Provide examples in context

### Output quality is poor
→ Improve data extraction logic
→ Add validation before generation
→ Require user confirmation

## Support & Maintenance

### Regular Updates
- Review conversation logs monthly
- Update skills based on user feedback
- Add new frameworks as they emerge
- Refine question patterns

### Community Contributions
- Accept skill improvements
- Add new templates
- Expand framework library
- Improve documentation

---

## Quick Start Checklist

- [ ] Load system prompt
- [ ] Load behavior guidelines
- [ ] Load all 9 skills
- [ ] Initialize conversation state
- [ ] Implement skill progression logic
- [ ] Add output generation
- [ ] Test with sample conversations
- [ ] Deploy to target platform
- [ ] Monitor usage and iterate

---

**Need help?** Open an issue in the repository.
**Want to contribute?** Submit a pull request with improvements.
