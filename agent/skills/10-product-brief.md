# Skill: Generate Product Brief

## Purpose
Transform validated business idea into a compelling one-page product brief that anyone from CEO to engineer can understand in 3 minutes. Channels Jeff Bezos's customer obsession and Steve Jobs's ruthless simplicity.

## When to Use
- User explicitly requests a "product brief"
- User needs a customer-facing narrative (not internal validation)
- User wants a concise pitch document after completing validation
- User says "prepare product brief" or similar

## Prerequisites
The product brief can be generated:
1. **After full validation** (Skills 1-8 completed) — best quality, uses all collected data
2. **Standalone** — user provides enough context directly (problem, solution, customer, differentiator)

If standalone, collect minimum required information before generating (see Required Information below).

## Conversation Flow

### If Called After Full Validation (Skills 1-8)
"I have all the validation data. Let me draft your product brief. This will be a one-page, customer-obsessed narrative — no jargon, no bullet lists, written as if you're launching today."

[Generate immediately from collected data]

### If Called Standalone
"Let's build your product brief. I need a few things first."

**Ask in sequence (stop as soon as you have enough):**

1. "What's the product name and what does it do in one sentence?"
2. "Who is it for? Be specific — role, company type, situation."
3. "What are the top 2 pain points your customer has today?"
4. "How does your product solve these? Describe the experience, not the features."
5. "Name 3 benefits the customer will remember."
6. "Why does this matter right now? What happens if they don't have it?"
7. "Do you have one data point or customer quote that proves the need?"

### Follow-up Probes (Socratic Method)

**Headline clarity:**
- "If you had to tweet this product in one line, what would you say?"
- "Would a stranger understand this in 5 seconds?"

**Customer obsession:**
- "Forget features — what transformation does the customer experience?"
- "If you were explaining this to Oprah, how would you describe it?"

**Simplicity check:**
- "Can you explain each benefit without using any industry jargon?"
- "Would your mom understand why this matters?"

**Urgency check:**
- "Why should someone care about this today, not next year?"
- "What's the cost of inaction?"

## Required Information

### Minimum (must have all)
- Product name
- Target customer (specific)
- Top 2 pain points
- How the product solves them
- 3 key benefits

### Ideal (adds quality)
- Why now / urgency
- Evidence (data point or customer quote)
- High-level concept / analogy
- Competitive differentiation

## Validation Checks
- [ ] Headline is Twitter-length (under 140 chars) and compelling
- [ ] Subheadline identifies WHO and WHAT transformation
- [ ] Pain points are customer problems, not feature gaps
- [ ] Solution is described as experience, not feature list
- [ ] Benefits use zero jargon — plain language only
- [ ] "Why Now" creates genuine urgency
- [ ] Evidence is concrete (number or direct quote)
- [ ] Total brief is under 300 words
- [ ] Reading it aloud sounds exciting, not boring
- [ ] Every sentence answers "So what?" from customer perspective

## Output Format

Use template: `/templates/product-brief-template.md`

**Structure:**
```
1. HEADLINE — Twitter-friendly product description
2. SUBHEADLINE — Who it's for + transformation
3. THE VILLAIN — Top 2 customer pain points (problems only)
4. THE HERO — How the product solves them (experience, not features)
5. THE MAGIC — Exactly 3 memorable benefits in plain language
6. WHY NOW? — Urgency + cost of inaction
7. THE EVIDENCE — One data point or customer quote
```

**Save to**: `/outputs/[sanitized-product-name]-product-brief.md`

## Agent Behavior

### Writing Style
- **Customer-obsessed**: Every word is about the customer's world, not yours
- **Ruthlessly simple**: If a 12-year-old can't understand it, rewrite it
- **Narrative, not lists**: Write in flowing prose (minimize bullet points)
- **Launch-day perspective**: Write as if the product is shipping today
- **Oprah-speak**: Explain it like you're on her couch — warm, clear, compelling

### Quality Rules
- Max 300 words total
- No jargon, acronyms, or technical terms
- No bullet lists unless absolutely essential
- Every sentence must answer "So what?" from customer perspective
- If it doesn't excite when read aloud, rewrite it
- Use ONLY information user provided or confirmed (ZERO hallucination)
- Mark any unvalidated claims

### Tone
- Confident but not arrogant
- Exciting but not hype-y
- Simple but not dumbed-down
- Customer-first, always

### After Generation
- Present the brief to user
- Ask: "Read this aloud. Does it excite you? Any section feel flat?"
- Offer to refine specific sections
- State filename clearly

## Relationship to Other Skills

### Uses Data From (if available)
- Skill 1 (Problem) → THE VILLAIN section
- Skill 2 (Customer Segments) → SUBHEADLINE + targeting
- Skill 3 (Value Proposition) → HEADLINE + THE HERO
- Skill 4 (Solution) → THE HERO + THE MAGIC
- Skill 5 (Market Validation) → THE EVIDENCE + WHY NOW
- Skill 7 (Key Metrics) → THE EVIDENCE
- Skill 8 (Risks) → Informs what NOT to overclaim

### Does NOT Replace
- Lean Canvas (internal validation document)
- Opportunity Assessment (strategic evaluation)
- These are complementary — product brief is the customer-facing narrative

## Examples

### Good Headline
- "MacBook Air: The world's thinnest notebook"
- "Slack: Where work happens"
- "Stripe: Payments infrastructure for the internet"

### Bad Headline
- "MacBook Air: A laptop with advanced thermal architecture and M-series chipset"
- "Slack: Enterprise communication and collaboration SaaS platform"
- "Stripe: RESTful API-based payment processing middleware"

### Good Villain (Pain Points)
"Field service teams arrive at job sites with outdated information. They waste hours calling back to the office for customer details, equipment history, and work instructions — while the customer watches and waits."

### Bad Villain
"Organizations lack a unified mobile-first CRM solution with offline-capable data synchronization and multi-backend connectivity."

## Next Skill
This is a terminal skill — no next skill. Returns to user with completed product brief.
