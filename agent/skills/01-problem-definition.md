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

**Collaborative approach**:
- **Accept and improve**: Take the answer, then suggest how to strengthen it
- **Help, don't block**: If too generic, guide toward specificity rather than rejecting
- **Mark assumptions**: If unvalidated, note it as assumption and move forward
- **Optional quantification**: Suggest metrics but don't require them

**Response patterns (helpful)**:
- **If generic**: "✓ Got it - [restate their answer]. Can you give a specific example to make this clearer?"
- **If vague**: "That's a start. What's one concrete pain point you've observed?"
- **If truly empty**: "Not sure? Let's try: Who has this problem? What frustrates them?"

**When to use Socratic questions** (optional, not mandatory):
- **"How do you know?"** → Only if claim seems unfounded, not for every answer
- **"Who specifically?"** → Only if they say "everyone" or "people"
- **"Can you quantify?"** → Suggest if possible, but accept qualitative answers

**When user lacks info**:
- Accept "I don't know" → Mark as TBD and move on
- Offer research: "Want me to look up common problems in [industry]?"
- Suggest estimation: "Make your best guess based on what you've seen."

**Examples**:
- ❌ "We make project management easier" → ✅ "Teams lose 5 hours/week manually tracking dependencies"
- ❌ "Help small businesses" → ✅ "10-50 person consultancies can't track billable hours accurately"
- ❌ "Better customer service" → ✅ "Support teams spend 30% of time searching for customer context"

### Next Skill
→ `02-customer-segments.md`
