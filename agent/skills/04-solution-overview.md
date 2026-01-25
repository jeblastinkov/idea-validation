# Skill: Solution Overview

## Purpose
Define minimum viable solution features.

## Conversation Flow

### Initial Question
"What are the top 3 features your MVP must have to solve this problem?"

### Follow-up Probes (Socratic Method)

**Constraint & Trade-off Questions**:
- "What's the simplest version that solves the core problem?" (avoid over-engineering)
- "If you had half the time/resources, what would you cut?" (reveals priorities)
- "What are we NOT going to do as part of the MVP?" (scope management)
- "What existing workflows does this disrupt?" (adoption barriers)

**Solution Validation Questions**:
- "Why is this the right solution for that problem?" (logical connection)
- "How will customers discover this solution?" (distribution thinking)
- "What would users pay for on day one?" (value test)
- "How will users access this?" (delivery channel)

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

### Agent Behavior (Socratic Approach)

**Challenge scope creep**:
- **If too many features**: "That's too much. If you had half the time, what would you cut first?"
- **If vague**: "Be specific. What exactly does this feature do? How does it solve the problem?"
- **If over-engineered**: "Can this be simpler? What's the fastest way to test the hypothesis?"

**Socratic Techniques**:
- **"Constraint Test"**: "If you could only build ONE feature, which one? Why?"
- **"Alternative Exploration"**: "What other ways could you solve this? Why did you choose this approach?"
- **"What Would Need to Be True"**: "What assumptions does this solution rely on? What needs to be true?"
- **"Second-Order Consequences"**: "If users adopt this, what changes in their workflow? What new problems emerge?"

**Red Flags**:
- ❌ "We need all these features to compete" → Likely scope creep
- ❌ "Our competitors have this so we need it" → Not user-driven
- ❌ "This will be easy to build" → Underestimating complexity

### Next Skill
→ `05-market-validation.md`
