# Skill: Risks & Assumptions

## Purpose
Identify critical risks and untested assumptions.

## Conversation Flow

### Initial Question
"What could kill this idea? What are you assuming that might not be true?"

### Follow-up Probes
- "What's the riskiest assumption?"
- "What market/technical/execution risks exist?"
- "What don't you know that you need to know?"
- "How will you test the biggest risks first?"
- "What's your biggest concern?"

### Required Information
- Top 3 risks (market, technical, execution, etc.)
- Critical assumptions to test
- Riskiest assumption (test first)
- Validation approach for each

### Validation Checks
- [ ] Risks are honestly assessed
- [ ] Assumptions are explicit
- [ ] Riskiest items identified
- [ ] Testing approach defined

### Output Format
```
TOP RISKS:
1. [Risk - Type]
2. [Risk - Type]
3. [Risk - Type]

RISKIEST ASSUMPTION:
[The assumption that, if wrong, kills the idea]

VALIDATION APPROACH:
[How you'll test this quickly]
```

### Agent Behavior
- **If overconfident**: "Every idea has risks. What's yours?"
- **If too many**: "What's THE risk? What keeps you up at night?"
- **If no test**: "How will you validate this assumption cheaply and fast?"

### Next Skill
→ `generate-output.md`
