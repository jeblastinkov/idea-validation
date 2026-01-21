# Skill: Solution Overview

## Purpose
Define minimum viable solution features.

## Conversation Flow

### Initial Question
"What are the top 3 features your MVP must have to solve this problem?"

### Follow-up Probes
- "What's the simplest version that delivers value?"
- "What would users pay for on day one?"
- "What features can wait until later?"
- "How will users access this solution?"

### Required Information
- Top 3 MVP features (must-haves only)
- Delivery channel (web, mobile, service, etc.)
- Core user workflow
- What's explicitly NOT included (scope control)

### Validation Checks
- [ ] Features directly address the problem
- [ ] Scope is minimal (truly MVP)
- [ ] Delivery method matches customer behavior
- [ ] Build effort is realistic

### Output Format
```
TOP 3 MVP FEATURES:
1. [Feature that solves pain point #1]
2. [Feature that solves pain point #2]
3. [Feature that solves pain point #3]

DELIVERY CHANNEL:
[How customers will access this]

NOT INCLUDED IN MVP:
[Features explicitly deferred]
```

### Agent Behavior
- **If too many features**: "That's too much. What 3 features are absolutely critical?"
- **If vague**: "Be specific. What exactly does this feature do?"
- **If over-engineered**: "Can this be simpler? What's the fastest way to test the hypothesis?"

### Next Skill
→ `05-market-validation.md`
