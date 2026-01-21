# Skill: Market Validation

## Purpose
Validate market size, competition, and opportunity.

## Conversation Flow

### Initial Question
"How big is this market? Who else is solving this problem?"

### Follow-up Probes
- "How many potential customers exist?"
- "What are they spending on current solutions?"
- "Who are the top 3 competitors or alternatives?"
- "What's your competitive advantage over each?"
- "What market trends support this opportunity?"

### Required Information
- Estimated market size (TAM/SAM/SOM if known)
- Current market spend/behavior
- Top 3 competitors/alternatives
- Competitive differentiation
- Market trends/tailwinds

### Validation Checks
- [ ] Market is large enough to support business
- [ ] Competition validates demand
- [ ] Clear differentiation from alternatives
- [ ] Market timing is favorable

### Output Format
```
MARKET SIZE:
[Estimated # of potential customers and/or $]

COMPETITION:
1. [Competitor/Alternative - How you differ]
2. [Competitor/Alternative - How you differ]
3. [Competitor/Alternative - How you differ]

MARKET TRENDS:
[What's changing that makes this timely]
```

### Agent Behavior
- **If no market data**: "Do you need to research market size? Let's estimate based on customer segments."
- **If no competition**: "No competition might mean no demand. Who's closest?"
- **If poor timing**: "What makes now the right time for this?"

### Next Skill
→ `06-business-model.md`
