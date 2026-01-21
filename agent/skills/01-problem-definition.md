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
- **If vague**: "Can you be more specific? What exactly frustrates users?"
- **If too broad**: "That's quite broad. Can you narrow it to a specific scenario?"
- **If no problem**: "Without a clear problem, validation can't proceed. Let's define what pain point this addresses."

### Next Skill
→ `02-customer-segments.md`
