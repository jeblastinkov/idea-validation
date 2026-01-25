# Skill: Problem Definition

## Purpose
Help users articulate the core problem their business idea solves.

## Conversation Flow

### Initial Question
"What problem does your idea solve?"

### Follow-up Probes (Socratic Method)

**Problem Clarity Questions**:
- "What specific pain point does this solve?" (concrete examples, not abstractions)
- "How do we know this is a real problem?" (evidence: interviews, data, observation)
- "Who experiences this problem most acutely?" (forces specificity)
- "What's the cost of NOT solving this?" (revenue loss, time waste, risk)
- "What do people do today when they have this problem?" (reveals alternatives)

**Evidence-Based Probes**:
- "How do you know?" (demand evidence)
- "Can you describe the last time this occurred?" (concrete instance)
- "How frequently does this problem occur?" (quantify)
- "How many people/companies experience this?" (scope)

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

**Response patterns (Socratic approach)**:
- **1st vague answer**: "Too vague. What SPECIFIC problem? Give a concrete example."
- **2nd vague answer**: "Still generic. Describe the last time this occurred. Who was affected? What happened?"
- **3rd vague answer**: "I need specifics. Tell me: What frustrates users? What breaks? What fails?"

**Socratic Probing Techniques**:
- **"What Would Need to Be True"**: "What would need to be true for this to be a major problem worth solving?"
- **"Second-Order Consequences"**: "If this problem persists, what happens? What cascade effects occur?"
- **"Evidence Check"**: "How do you know this? What evidence do you have? Who told you?"
- **"Steel Man Counter"**: "Some might argue this problem isn't painful enough to pay for. How would you respond?"

**When user lacks info**:
- If user says "I don't know": "Can you estimate based on observation? Who have you talked to?"
- If still stuck: "Who is your target customer? What industry? Let me research common problems in that space."
- Use WebSearch to find industry pain points
- Present: "In [industry], common problems are [X, Y, Z]. Which resonates?"

**Examples**:
- ❌ "We make project management easier" → ✅ "Teams lose 5 hours/week manually tracking dependencies"
- ❌ "Help small businesses" → ✅ "10-50 person consultancies can't track billable hours accurately"
- ❌ "Better customer service" → ✅ "Support teams spend 30% of time searching for customer context"

### Next Skill
→ `02-customer-segments.md`
