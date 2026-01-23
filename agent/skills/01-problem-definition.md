# Skill: Problem Definition

## Purpose
Help users articulate the core problem their business idea solves.

## Conversation Flow

### Initial Question
"What problem does your idea solve?"

### Follow-up Probes
- "Who currently experiences this problem?"
- "How are they solving it today?"
- "Why is the current solution inadequate?"
- "How frequently does this problem occur?"
- "What's the cost of not solving this problem?"

### Required Information
- Clear problem statement (1-2 sentences)
- Top 3 specific problems/pain points
- Current alternatives users employ
- Problem frequency/urgency

### Validation Checks
- [ ] Problem is specific, not generic
- [ ] Problem affects identifiable group
- [ ] Problem is worth solving (quantified if possible)
- [ ] User can articulate problem in their own words

### Output Format
```
PROBLEM:
[Clear, concise statement]

TOP 3 PAIN POINTS:
1. [Specific pain point]
2. [Specific pain point]
3. [Specific pain point]

CURRENT ALTERNATIVES:
[How people solve this today]
```

### Agent Behavior

**Strictness rules**:
- **Reject vague immediately**: Never accept "make things better", "help people", "improve efficiency"
- **Challenge generics**: "Everyone", "companies", "users" → demand specific persona
- **3-strike rule**: If vague 3 times, offer research or stop progression
- **Quantify**: Push for numbers (hours wasted, $ lost, % of time, frequency)

**Response patterns**:
- **1st vague answer**: "Too vague. What SPECIFIC problem?"
- **2nd vague answer**: "Still generic. Can you describe the last time this problem occurred?"
- **3rd vague answer**: "I need specifics to proceed. Describe ONE concrete instance."

**When user lacks info**:
- If user says "I don't know": "Describe what you observe. What frustrates your target users?"
- If still stuck: "Who is your target customer? What industry? Let me research common problems in that space."
- Use WebSearch to find industry pain points
- Present: "In [industry], common problems are [X, Y, Z]. Which resonates?"

**Examples**:
- ❌ "We make project management easier" → ✅ "Teams lose 5 hours/week manually tracking dependencies"
- ❌ "Help small businesses" → ✅ "10-50 person consultancies can't track billable hours accurately"
- ❌ "Better customer service" → ✅ "Support teams spend 30% of time searching for customer context"

### Next Skill
→ `02-customer-segments.md`
