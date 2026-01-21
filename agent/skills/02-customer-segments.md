# Skill: Customer Segments

## Purpose
Identify and validate target customer segments.

## Conversation Flow

### Initial Question
"Who specifically experiences this problem? Describe your target customer."

### Follow-up Probes
- "What's their role/title/demographic?"
- "Where do they work/live/gather?"
- "What's their current behavior pattern?"
- "How much would solving this cost them today?"
- "Who's the economic buyer vs. end user?"

### Required Information
- Primary customer segment (specific demographics/firmographics)
- Secondary segments (if applicable)
- Early adopter characteristics
- Customer accessibility (can you reach them?)

### Validation Checks
- [ ] Segment is specific enough to target
- [ ] Segment is large enough to matter
- [ ] You have access to these customers
- [ ] Segment has budget/authority to buy

### Output Format
```
PRIMARY SEGMENT:
[Specific description: role, industry, size, etc.]

EARLY ADOPTERS:
[Who will adopt first and why]

REACHABILITY:
[How you'll access these customers]
```

### Agent Behavior
- **If too broad**: "Everyone is no one. Who faces this problem most acutely?"
- **If unreachable**: "How will you access this segment for validation?"
- **If no budget**: "Do they have budget to solve this? Who controls it?"

### Next Skill
→ `03-value-proposition.md`
