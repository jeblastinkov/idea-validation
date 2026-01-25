# Socratic Questioning Integration Guide

**Version**: 1.0
**Date**: 2026-01-25
**Purpose**: Guide to using Socratic questioning methodology with Lean Canvas and SVPG frameworks

---

## Overview

This guide explains how Socratic questioning has been integrated into the idea validation agent to provide deeper, more rigorous validation conversations.

## What is Socratic Questioning?

Socratic questioning is a method of disciplined, thoughtful dialogue that uses targeted questions to:
- Uncover hidden assumptions
- Clarify vague or fuzzy thinking
- Surface potential issues before they become problems
- Strengthen the reasoning behind business decisions

**Key principle**: The goal is NOT to challenge or interrogate, but to help founders think more clearly.

---

## The 5 Socratic Question Categories

### 1. Problem Clarity Questions
**Purpose**: Ensure the problem is real and well-understood

**Key questions**:
- "What specific pain point does this solve?"
- "How do we know this is a real problem?"
- "Who experiences this problem most acutely?"
- "What's the cost of NOT solving this?"
- "What do people do today when they have this problem?"

**Example in action**:
```
❌ Weak: "We make project management easier"
Agent: "Too vague. What SPECIFIC problem in project management?"
User: "Teams waste time tracking dependencies manually"
Agent: "How much time? How do you know?"
User: "Our team spends 5 hours/week updating spreadsheets"
✅ Strong: "Teams waste 5 hours/week manually tracking cross-project dependencies"
```

### 2. Solution Validation Questions
**Purpose**: Ensure the proposed solution actually solves the problem

**Key questions**:
- "Why is this the right solution for that problem?"
- "What alternatives did you consider? Why did you reject them?"
- "What's the simplest version that solves the core problem?"
- "How will customers discover this solution?"
- "What would need to be true for this solution to work?"

**Example in action**:
```
User: "We'll build an AI-powered dashboard"
Agent: "Why AI specifically? What alternatives did you consider?"
User: "Well, we could do manual tracking or use existing tools"
Agent: "Why did you reject existing tools?"
User: "They don't auto-detect dependencies across repos"
✅ Clear differentiation: AI auto-detection vs manual configuration
```

### 3. Success Criteria Questions
**Purpose**: Ensure we can measure if the solution works

**Key questions**:
- "How will we know if this idea is successful?"
- "What would make you consider this idea a failure?"
- "What metric are we trying to move? By how much?"
- "What customer behavior change are we looking for?"
- "What's the adoption target for the first 6 months?"

**Example in action**:
```
User: "We'll get lots of users"
Agent: "What metric? What target?"
User: "Um, maybe 10,000 signups?"
Agent: "Signups don't equal success. What behavior shows real value?"
User: "Daily active usage of the dependency tracker"
Agent: "What's the target? What percentage of signups become daily active?"
✅ Clear metric: 30% of signups become daily active users within 2 weeks
```

### 4. Constraint & Trade-off Questions
**Purpose**: Surface limitations and difficult decisions

**Key questions**:
- "What are the technical or operational constraints?"
- "What are we NOT going to do as part of the MVP?"
- "What existing solutions or workflows does this disrupt?"
- "If you had half the time/resources, what would you cut?"
- "What would you need to believe to 10x the price?"

**Example in action**:
```
User: "We'll have auto-detection, ML suggestions, analytics, integrations, and custom workflows"
Agent: "That's too much. If you had half the time, what would you cut?"
User: "Probably custom workflows and analytics"
Agent: "What are the top 3 features that solve the core problem?"
✅ Focused MVP: Auto-detection, visual graph, Slack alerts
```

### 5. Strategic Fit Questions
**Purpose**: Ensure idea aligns with market opportunity and founder capabilities

**Key questions**:
- "Why is this the right idea to pursue RIGHT NOW?"
- "Why are you uniquely positioned to build this?"
- "What happens if you wait 6 months to build this?"
- "How does this idea change in a best-case vs worst-case scenario?"
- "What would make this a billion-dollar vs million-dollar business?"

**Example in action**:
```
User: "This could be huge!"
Agent: "Why are YOU uniquely positioned to build this?"
User: "I've been an engineering manager for 10 years and felt this pain daily"
Agent: "✓ Domain expertise. Why now? What's changed?"
User: "GitHub's new dependency API makes auto-detection possible"
✅ Clear timing: New technology enables solution that wasn't possible before
```

---

## How Socratic Questions Map to Frameworks

### Lean Canvas Integration

| Lean Canvas Section | Primary Socratic Category | Example Questions |
|---------------------|---------------------------|-------------------|
| **Problem** | Problem Clarity | "What specific pain? Who has it? How do you know?" |
| **Customer Segments** | Problem Clarity + Strategic Fit | "Who most acutely? How reachable? Why you?" |
| **Unique Value Proposition** | Solution Validation | "Why this solution? What alternatives exist?" |
| **Solution** | Solution Validation + Constraints | "Simplest version? What's not included?" |
| **Channels** | Solution Validation | "How will they discover it?" |
| **Revenue Streams** | Success Criteria + Constraints | "What would you pay? What drives 10x price?" |
| **Cost Structure** | Constraints | "Key costs? Unit economics?" |
| **Key Metrics** | Success Criteria | "What metric? What target?" |
| **Unfair Advantage** | Strategic Fit | "Why you? Why now? What's unique?" |

### SVPG Opportunity Assessment Integration

| SVPG Question | Primary Socratic Category | Enhanced Questions |
|---------------|---------------------------|-------------------|
| **What problem?** | Problem Clarity | "Specific pain? Evidence? Cost of not solving?" |
| **For whom?** | Problem Clarity | "Who most acutely? How many? How reachable?" |
| **How big?** | Success Criteria + Strategic Fit | "TAM/SAM/SOM? What makes this huge?" |
| **What alternatives?** | Solution Validation | "What exists? Why not good enough?" |
| **Why us?** | Strategic Fit | "Unfair advantage? Unique positioning?" |
| **Why now?** | Strategic Fit | "What's changed? What if we wait?" |
| **How to reach?** | Solution Validation | "Discovery? Channels? Distribution?" |
| **Success metrics?** | Success Criteria | "What metric? Target? Behavior change?" |
| **What must go right?** | Constraints | "Critical assumptions? Dependencies?" |
| **What risks?** | Constraints | "Value? Usability? Feasibility? Viability?" |

---

## Agent Behavior Changes

### Before Socratic Integration

**Old approach**:
- Ask question
- Accept vague answer
- Move on
- Generate canvas with assumptions

**Problems**:
- Weak validation
- Unexamined assumptions
- Generic outputs
- Low confidence in results

### After Socratic Integration

**New approach**:
- Ask question
- **If vague**: Probe deeper with Socratic techniques
- **If unsupported**: Challenge with evidence requests
- **If generic**: Force specificity with follow-ups
- **If weak**: Use 3-strike rule, then research or block

**Benefits**:
- Rigorous validation
- Explicit assumptions
- Specific, concrete outputs
- High confidence in results

---

## Socratic Techniques in Practice

### Technique 1: "What Would Need to Be True"

**Purpose**: Surface assumptions without direct confrontation

**Pattern**:
```
Instead of: "Will customers pay $100/month?"
Ask: "What would need to be true for customers to pay $100/month?"
```

**Example**:
```
Agent: "What would need to be true for enterprise customers to pay $500/user/month?"
User: "They'd need to save at least $2,000/user/month in productivity"
Agent: "How will you prove that savings? What metrics will you track?"
✅ Assumption surfaced: 4x ROI required, needs productivity measurement
```

### Technique 2: "Steel Man Counter-Argument"

**Purpose**: Test resilience of thinking by presenting strongest opposing view

**Pattern**:
```
Present strongest counter-argument
Ask how founder would respond
Reveals blind spots or strengthens reasoning
```

**Example**:
```
Agent: "The strongest argument against this is that incumbents will copy your feature in 6 months. How do you respond?"
User: "Good point. But we have 2 years of proprietary training data they can't replicate"
✅ Defensibility clarified: Data moat, not just feature advantage
```

### Technique 3: "Second-Order Consequences"

**Purpose**: Think beyond the first success to what happens next

**Pattern**:
```
Instead of: "Will this succeed?"
Ask: "If you succeed, what happens next?"
```

**Example**:
```
Agent: "If you get 10,000 users, what's the next bottleneck?"
User: "Hmm, probably customer support. Each user needs onboarding"
Agent: "Can the business model support that support cost?"
✅ Reveals scaling issue: High-touch model may not work at scale
```

### Technique 4: "Evidence Check"

**Purpose**: Ensure claims are supported by data, not assumptions

**Pattern**:
```
Challenge: "How do you know?"
Follow-up: "What evidence supports that?"
Probe: "Who told you this? When?"
```

**Example**:
```
User: "The market is $10B"
Agent: "How do you know? What's your source?"
User: "I read it somewhere"
Agent: "Let me research that. [WebSearch] Found $6B (Gartner 2024). Confirm?"
✅ Fact-checked: Corrected market size with authoritative source
```

### Technique 5: "Alternative Exploration"

**Purpose**: Ensure multiple options were considered

**Pattern**:
```
Ask: "What alternatives did you consider?"
Probe: "Why did you reject [obvious alternative]?"
Challenge: "This seems like the only option - is that true?"
```

**Example**:
```
Agent: "What alternatives to building custom AI did you consider?"
User: "Just using OpenAI API"
Agent: "Why did you reject that?"
User: "Data privacy - our customers can't send data to external APIs"
✅ Clear reasoning: Compliance requirement drives build vs buy decision
```

---

## Red Flags the Agent Listens For

### 1. Vague Language
- "People want better..." → Demand: "What specifically? Which people?"
- "This will improve..." → Demand: "Improve what? By how much?"
- "Everyone needs..." → Challenge: "Really? Everyone? Who most acutely?"

### 2. Solution-First Thinking
- Can describe product but not problem → Probe: "What problem does this solve?"
- "Competitors have it" as justification → Challenge: "Why do YOUR customers need it?"

### 3. Lack of Evidence
- "I think customers would..." → Demand: "How do you know? What evidence?"
- Only anecdotes → Probe: "How many people have this problem?"

### 4. Unclear Success Criteria
- Can't articulate success → Force: "What metric? What target?"
- No timeline → Demand: "Success in 6 months looks like what?"

### 5. Unfounded Optimism
- "We'll capture 1% of huge market" → Challenge: "How specifically will you reach them?"
- "Build it and they will come" → Probe: "How will they discover it?"

---

## Conversation Flow Examples

### Example 1: Problem Definition (Socratic Approach)

```
Agent: What problem does your idea solve?

User: We help companies manage projects better.

Agent: Too generic. What specific pain point? What's broken in current project management?

User: Development teams can't track dependencies across projects.

Agent: ✓ More specific. How do you know this is a real problem? What evidence?

User: I'm an engineering manager and I see it daily.

Agent: How much time does this waste? Can you quantify?

User: Teams spend about 5 hours per week manually updating dependency spreadsheets.

Agent: ✓ Quantified. Who experiences this most acutely? What size teams?

User: Engineering managers at companies with 50-200 engineers, multiple teams working on related services.

Agent: ✓ Clear target. What's the cost of NOT solving this? What happens when dependencies aren't tracked?

User: Deployment conflicts, blocked teams, missed deadlines. Probably costs 20-30 hours of engineering time per incident.

Agent: ✓ Strong problem statement. Moving to customer segments.
```

**Socratic techniques used**:
- Problem Clarity: "What specific pain point?"
- Evidence Check: "How do you know this is real?"
- Quantification: "How much time?"
- Specificity: "Who most acutely?"
- Consequence Probing: "What's the cost of NOT solving?"

### Example 2: Solution Validation (Socratic Approach)

```
Agent: What's your solution? Top 3 MVP features?

User: AI-powered project management platform with scheduling, resource allocation, risk prediction, collaboration tools, time tracking, and reporting.

Agent: That's too much. If you had half the time and resources, what would you cut?

User: Probably time tracking and advanced reporting.

Agent: What about the remaining features? What's the simplest version that solves the dependency tracking problem?

User: Auto-detect dependencies, visualize them, alert on conflicts.

Agent: ✓ That's focused. Why AI specifically? What alternatives did you consider?

User: We could do manual dependency mapping, but that's what exists today. AI auto-detection from code is the differentiator.

Agent: How will teams discover this tool? How does it integrate into their workflow?

User: GitHub app that runs on PRs and posts to Slack.

Agent: ✓ Clear distribution. What would need to be true for teams to actually use this vs ignore the Slack notifications?

User: The alerts would need to be accurate (low false positives) and actionable (clear what to do).

Agent: ✓ Critical assumptions identified. How will you validate accuracy before launch?

User: Test on our own codebase first, aim for 90%+ accuracy.

Agent: ✓ Validation plan clear. Moving to metrics.
```

**Socratic techniques used**:
- Constraint Test: "If you had half the time, what would you cut?"
- Alternative Exploration: "What alternatives did you consider?"
- Solution Validation: "How will they discover this?"
- "What Would Need to Be True": "What needs to be true for adoption?"
- Evidence Check: "How will you validate accuracy?"

---

## Implementation in Agent Skills

Each of the 9 agent skills has been enhanced with Socratic questioning:

### Skill 1: Problem Definition
- Uses Problem Clarity questions
- Demands evidence with Evidence Check
- Quantifies with "How much?" probes
- Tests understanding with Second-Order Consequences

### Skill 2: Customer Segments
- Uses Problem Clarity for "Who most acutely?"
- Uses Strategic Fit for "Why you?" and "How reachable?"

### Skill 3: Value Proposition
- Uses Solution Validation for differentiation
- Uses Strategic Fit for "Why now?" and unfair advantage
- Uses Steel Man Counter for competitive threats

### Skill 4: Solution Overview
- Uses Constraints questions for MVP scoping
- Uses "What Would Need to Be True" for assumptions
- Uses Alternative Exploration for solution validation

### Skill 5: Market Validation
- Uses Strategic Fit for market timing
- Uses Evidence Check for market size claims
- Research capability for TAM/SAM/SOM validation

### Skill 6: Business Model
- Uses Success Criteria for pricing validation
- Uses Constraints for cost structure
- Uses "What Would Need to Be True" for unit economics

### Skill 7: Key Metrics
- Uses Success Criteria questions exclusively
- Challenges vanity metrics
- Demands behavior change metrics

### Skill 8: Risks & Assumptions
- Synthesizes all Socratic categories
- Uses "What Would Need to Be True" extensively
- Identifies riskiest assumption for testing

### Skill 9: Generate Output
- Compiles all Socratic insights
- Cites researched evidence
- Marks untested assumptions clearly

---

## Quality Improvement

### Before Socratic Integration

**Example weak output**:
```
PROBLEM: Project management is hard
CUSTOMER: Companies
SOLUTION: Better project management software
METRIC: Users
RISK: Competition
```

**Issues**:
- Vague, generic statements
- No specificity
- No evidence
- No validation plan

### After Socratic Integration

**Example strong output**:
```
PROBLEM: Engineering teams (50-200 engineers) waste 5 hours/week manually tracking cross-project dependencies in spreadsheets, leading to deployment conflicts and 20-30 hours of recovery time per incident.

CUSTOMER: Engineering managers at B2B SaaS companies with microservices architecture, 50-200 engineers, primarily US-based tech companies.

SOLUTION: GitHub app that auto-detects dependencies from code, visualizes dependency graph, and alerts in Slack when conflicts are detected. NOT including: time tracking, advanced analytics, CRM integration (deferred to V2).

METRIC: 30% of installations become daily active users within 2 weeks (defined as checking dependency graph or acting on alerts daily). Validation: 90%+ accuracy on dependency detection in pilot with 5 teams.

RISK: Riskiest assumption is that teams will trust AI-generated dependency detection. Validation: Manual review comparison with 90%+ accuracy threshold required before launch.
```

**Improvements**:
- Specific, quantified problem
- Clear target customer
- Focused, scoped solution
- Measurable success criteria
- Testable assumptions

---

## Best Practices for Using Socratic Approach

### For Founders/Users

**Do**:
- ✅ Expect to be challenged on vague statements
- ✅ Provide concrete examples when possible
- ✅ Share evidence (user interviews, data, personal experience)
- ✅ Be honest about unknowns - say "I don't know" when you don't know
- ✅ Think through alternatives before dismissing them

**Don't**:
- ❌ Take challenges personally - the goal is clarity, not criticism
- ❌ Provide generic "everyone" or "people" answers
- ❌ Claim market data without sources
- ❌ Avoid admitting assumptions - they're expected and important

### For Agent/Implementers

**Do**:
- ✅ Pick 3-5 most relevant Socratic questions per skill
- ✅ Use techniques to uncover assumptions, not to interrogate
- ✅ Offer research when user lacks critical data
- ✅ Acknowledge strong answers before moving on
- ✅ Use 3-strike rule to prevent endless back-and-forth

**Don't**:
- ❌ Ask all questions - prioritize most important
- ❌ Make users defensive with "gotcha" questions
- ❌ Skip evidence gathering for critical claims
- ❌ Accept vague answers just to move forward
- ❌ Hallucinate data - mark unknowns as "TBD"

---

## Outcomes & Benefits

### For Individual Founders

**Before Socratic approach**:
- Vague ideas
- Hidden assumptions
- Weak validation
- Low confidence

**After Socratic approach**:
- Clear, specific ideas
- Explicit assumptions
- Rigorous validation
- High confidence in next steps

### For Teams

**Before**:
- Misalignment on problem/solution
- Unspoken assumptions
- Unclear priorities
- Debate over metrics

**After**:
- Shared understanding of problem
- Documented assumptions
- Clear MVP scope
- Agreed success criteria

### For Investors/Stakeholders

**Before**:
- Generic pitch
- Unvalidated claims
- No evidence
- Unclear differentiation

**After**:
- Specific, evidence-based pitch
- Validated assumptions (or marked for testing)
- Data-driven claims
- Clear competitive advantage

---

## Conclusion

Socratic questioning transforms idea validation from a form-filling exercise into rigorous, evidence-based thinking. By integrating these techniques into the Lean Canvas and SVPG frameworks, founders get:

1. **Deeper clarity** on problems, solutions, and assumptions
2. **Better evidence** through research and validation
3. **Stronger outputs** that are specific, testable, and actionable
4. **Higher confidence** in their next steps

**Remember**: The goal is not to be difficult or challenging, but to help founders think clearly and build something that actually solves a real problem for real customers.

---

## References

- **Socratic Questioning Framework**: `/frameworks/socratic-questioning.md`
- **Agent Behavior Guidelines**: `/agent/behavior-guidelines.md`
- **Enhanced Skills**: `/agent/skills/01-09-*.md`
- **Framework Comparison**: `/frameworks/comparison.md`

---

**Questions or feedback?** Update this guide as you learn what works and what doesn't. Socratic questioning is a practice that improves with use.
