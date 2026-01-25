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

**Balanced approach**: Accept, then challenge once to improve

**Response patterns**:
- **If generic**: "✓ Got it - [restate]. But what SPECIFICALLY? [Targeted question]"
  - Example: "✓ Better productivity. But what specific task takes too long?"
- **If vague**: "✓ [Confirm]. Can you quantify that? How many hours/dollars?"
  - Example: "✓ Waste time on research. How many hours per week?"
- **If missing evidence**: "✓ Noted. How do you know this? Have you seen it personally?"
  - Example: "✓ PMs struggle with this. Is that from your experience or observation?"

**Use Socratic challenges actively** (but don't block):
- **"Everyone"** → "✓ Broad. Who needs this MOST? Which segment?"
- **No quantification** → "✓ Got it. Can you estimate? Ballpark hours or dollars?"
- **Unsupported claim** → "✓ Interesting. How do you know? What's the evidence?"

**If they improve**: "✓ Much clearer. [Restate improved answer]. Moving on."
**If they can't/won't**: "✓ Marking as assumption to validate. Moving on."

**When user says "I don't know"**:
- Ask: "Can you estimate based on your experience?"
- If no: "Want me to research common [industry] problems?"
- If still no: "✓ Marking as TBD. Moving on."

**Examples**:
- ❌ "We make project management easier" → ✅ "Teams lose 5 hours/week manually tracking dependencies"
- ❌ "Help small businesses" → ✅ "10-50 person consultancies can't track billable hours accurately"
- ❌ "Better customer service" → ✅ "Support teams spend 30% of time searching for customer context"

### Next Skill
→ `02-customer-segments.md`
