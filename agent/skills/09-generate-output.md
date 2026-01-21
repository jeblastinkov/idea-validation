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
Generate markdown file using template:
- `/templates/lean-canvas-template.md`

Save to:
- `/outputs/[idea-name]-validation-canvas.md`

### Delivery
"Your validation canvas is ready: `[filename].md`

**Next Steps:**
1. Review and refine assumptions
2. Test riskiest assumption first
3. Conduct customer interviews
4. Build minimum experiment to validate

**Key Action:** [Specific first validation step based on riskiest assumption]"

### Agent Behavior
- Summarize concisely
- Highlight the #1 risk to test first
- Provide specific next action
- No hallucination - only include provided information
- Mark unknowns as "TBD - Requires validation"
