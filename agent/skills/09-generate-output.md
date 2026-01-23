# Skill: Generate Output

## Purpose
Compile validation into one-page Lean Canvas.

## Process

### Data Compilation
Gather all information from previous skills:
1. Problem Definition
2. Customer Segments
3. Value Proposition
4. Solution Overview
5. Market Validation
6. Business Model
7. Key Metrics
8. Risks & Assumptions

### Final Review
"I've gathered all the information. Let me create your one-page validation canvas. Review the summary:"

[Present condensed overview of all sections]

"Does this accurately reflect your idea? Any changes?"

### Output Generation

**Select template**:
- Lean Canvas: `/templates/lean-canvas-template.md` (150-200 lines target)
- SVPG Assessment: `/templates/opportunity-assessment-template.md` (250-300 lines target)

**Generate file**:
1. Use ONLY user-provided + researched (confirmed) data
2. Add executive summary at top (5-line overview)
3. Format professionally (scannable, bullets, short paragraphs)
4. Cite sources for researched data: "(Source: X via WebSearch)"
5. Mark unknowns: "TBD - Requires validation"
6. No duplication - each point stated once
7. Check length: Lean 150-200, SVPG 250-300

**Save to**: `/outputs/[sanitized-idea-name]-validation-canvas.md` or `-opportunity-assessment.md`

### Delivery
"Your validation canvas is ready: `[filename].md`

**Next Steps:**
1. Review and refine assumptions
2. Test riskiest assumption first
3. Conduct customer interviews
4. Build minimum experiment to validate

**Key Action:** [Specific first validation step based on riskiest assumption]"

### Agent Behavior

**Quality checklist before generating**:
- [ ] All 8 skills completed (Lean) or 10 questions (SVPG)
- [ ] No vague statements remain ("everyone", "better", etc.)
- [ ] Quantified where possible (market size, pricing, timelines)
- [ ] Assumptions explicitly marked as "TBD"
- [ ] Researched data cited with sources
- [ ] User confirmed summary

**Content rules**:
- Use ONLY provided/researched information (ZERO hallucination)
- Mark unknowns as "TBD - Requires validation"
- Cite researched data: "(Source: [X] via WebSearch, 2024)"
- No embellishment or invented context

**Executive formatting**:
- Executive summary at top (Decision, risks, next action)
- Scannable structure (bullets, short paragraphs max 4 lines)
- Concise sections (10-30 lines each)
- Professional tone (no emojis unless requested)
- Length within target (150-200 Lean, 250-300 SVPG)

**After generation**:
- Highlight #1 riskiest assumption
- Provide ONE specific next action (with timeframe)
- No congratulations or cheerleading
- State filename clearly
