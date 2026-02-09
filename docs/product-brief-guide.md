# Product Brief Guide

## What Is a Product Brief?

A one-page, customer-obsessed product narrative (~300 words) that anyone from CEO to engineer can understand in 3 minutes. Inspired by Jeff Bezos's customer obsession and Steve Jobs's ruthless simplicity.

**It is NOT** a business model, validation canvas, or strategic assessment. It complements those documents by providing the customer-facing story.

## When to Use

| Scenario | Use Product Brief? |
|----------|-------------------|
| Aligning team on product vision | Yes |
| Investor pitch prep | Yes |
| Marketing brief input | Yes |
| Product launch narrative | Yes |
| Validating a business idea | No — use Lean Canvas |
| Evaluating strategic fit | No — use Opportunity Assessment |
| Deep customer research | No — use Value Proposition Canvas |

## How to Request

Simply ask the agent:

- "Prepare a product brief"
- "Create a product brief for [product name]"
- "Generate a product brief" (after completing validation)

The agent will either:
1. **Use existing validation data** (if Skills 1-8 are completed) — generates immediately
2. **Ask minimum questions** (if standalone) — collects product name, customer, pain points, solution, and 3 benefits before generating

## Structure

The product brief follows a 7-section narrative structure:

### 1. HEADLINE (1 line)
Twitter-friendly product description.
Format: `"[Product Name]: [One compelling benefit]"`

**Good**: "MacBook Air: The world's thinnest notebook"
**Bad**: "MacBook Air: A laptop with advanced thermal architecture and M-series chipset"

### 2. SUBHEADLINE (1 sentence)
Who it's for and the transformation it delivers.

### 3. THE VILLAIN (2-3 sentences)
The customer's top 2 pain points. Focus only on problems — no solutions yet. Make the reader feel the frustration.

### 4. THE HERO (2-3 sentences)
How the product elegantly solves these problems. Focus on customer experience, not features. Use "Oprah-speak" — explain it like you're on her couch.

### 5. THE MAGIC (Rule of 3)
Exactly 3 key benefits customers will remember. Each in plain language with zero jargon.

### 6. WHY NOW? (1-2 sentences)
Why this matters today. What happens if customers don't have this.

### 7. THE EVIDENCE (brief)
One concrete data point or customer quote that validates the need.

## Writing Rules

1. **Max 300 words** — if it's longer, cut ruthlessly
2. **No jargon, acronyms, or technical terms** — if your mom can't understand it, rewrite
3. **No bullet lists** unless absolutely essential — use flowing prose
4. **Write from launch day** — as if the product already exists
5. **Every sentence answers "So what?"** from the customer's perspective
6. **Read it aloud** — if it doesn't excite you, rewrite it

## Files

| File | Purpose |
|------|---------|
| `agent/skills/10-product-brief.md` | Skill definition — conversation flow, probes, validation checks |
| `templates/product-brief-template.md` | Output template — the structure the generated brief follows |
| `outputs/[name]-product-brief.md` | Generated output — saved here |

## Relationship to Other Outputs

```
Lean Canvas (internal validation)
    ↓ data feeds into
Product Brief (customer-facing narrative)
    ↓ informs
Marketing copy, pitch decks, team alignment
```

The product brief draws from validation data but tells it as a customer story. It's the bridge between internal analysis and external communication.

## Example Flow

### After Full Validation
```
User: "Now prepare a product brief"
Agent: [Generates immediately from collected Skills 1-8 data]
Agent: "Your product brief is ready: outputs/acme-widget-product-brief.md
        Read it aloud. Does it excite you? Any section feel flat?"
```

### Standalone
```
User: "Prepare a product brief for our new field service app"
Agent: "What's the product name and what does it do in one sentence?"
User: "FieldPro — mobile app for field technicians to manage work orders offline"
Agent: "Who specifically is this for?"
User: "Field service managers at utilities companies, 500+ employees"
Agent: "Top 2 pain points they have today?"
...
[After collecting minimum info]
Agent: [Generates product brief]
```

## Quality Checklist

Before finalizing, verify:
- [ ] Headline is Twitter-length and compelling
- [ ] A stranger can understand the subheadline in 5 seconds
- [ ] The Villain makes you feel the customer's pain
- [ ] The Hero describes experience, not features
- [ ] All 3 Magic benefits use zero jargon
- [ ] "Why Now" creates genuine urgency
- [ ] Evidence is a real number or real quote
- [ ] Total is under 300 words
- [ ] It excites you when read aloud
