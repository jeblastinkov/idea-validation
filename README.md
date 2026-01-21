# Business Idea Validation Agent

A conversational AI agent that guides product managers and product leaders through structured business idea validation using proven methodologies like Lean Canvas and SVPG Product Discovery.

## What It Does

This agent helps you:
- **Define the problem** you're solving clearly
- **Identify target customers** specifically
- **Validate your value proposition** and differentiation
- **Assess market opportunity** and competition
- **Design business model** and pricing
- **Identify critical risks** and assumptions to test
- **Generate a one-page validation canvas** as output

## Why Use It

- ✅ **Structured approach**: Follows proven validation frameworks
- ✅ **Prevents hallucination**: Only uses information you provide
- ✅ **Challenges assumptions**: Pushes for clarity and evidence
- ✅ **Brief and direct**: Executive-level communication
- ✅ **Actionable output**: One-page canvas with next steps
- ✅ **Risk-focused**: Identifies riskiest assumptions to test first

## Quick Start

### 1. Clone or Download
```bash
git clone <repository-url>
cd idea-validation
```

### 2. Review the Framework
Read `/frameworks/lean-canvas.md` to understand the methodology.

### 3. Use the Agent

The agent guides you through 8 validation skills:

1. **Problem Definition** - What problem are you solving?
2. **Customer Segments** - Who has this problem?
3. **Value Proposition** - What makes you different?
4. **Solution Overview** - What will you build?
5. **Market Validation** - How big is the opportunity?
6. **Business Model** - How will you make money?
7. **Key Metrics** - How will you measure success?
8. **Risks & Assumptions** - What could go wrong?

### 4. Get Your Output

After completing all skills, the agent generates a one-page validation canvas saved to `/outputs/[your-idea]-validation-canvas.md`.

## Agent Behavior

### What to Expect

**Brief Responses**
```
Agent: "What problem does your idea solve?"
```

**Direct Challenges**
```
User: "Our target market is small businesses."
Agent: "Too broad. Which specific type? What size? What industry?"
```

**No Hallucination**
```
Agent: "Need market size. Estimate or mark as TBD?"
(Instead of making up numbers)
```

### Communication Style

- **2-3 sentences max** per response
- **Asks for specifics** when answers are vague
- **Challenges assumptions** respectfully
- **Marks unknowns** as "TBD - Requires validation"
- **Provides specific next action** after completion

## Project Structure

```
/
├── README.md                          # This file
├── agent/
│   ├── system-prompt.md              # Core agent instructions
│   ├── behavior-guidelines.md        # Detailed behavior rules
│   ├── agent-config.md               # Configuration
│   ├── implementation-guide.md       # How to implement
│   └── skills/                        # 9 conversation skills
│       ├── 01-problem-definition.md
│       ├── 02-customer-segments.md
│       ├── 03-value-proposition.md
│       ├── 04-solution-overview.md
│       ├── 05-market-validation.md
│       ├── 06-business-model.md
│       ├── 07-key-metrics.md
│       ├── 08-risks-assumptions.md
│       └── 09-generate-output.md
├── frameworks/
│   ├── lean-canvas.md                # Lean Canvas guide
│   ├── opportunity-assessment.md     # SVPG framework
│   └── comparison.md                 # When to use which
├── templates/
│   ├── lean-canvas-template.md       # Output template
│   ├── opportunity-assessment-template.md
│   └── output-onepager-template.md
├── outputs/                           # Generated canvases
└── docs/
    ├── methodology-guide.md
    └── getting-started.md
```

## Methodologies

This agent is based on:

### Lean Canvas
- **Created by**: Ash Maurya
- **Purpose**: One-page business model for startups
- **When**: Validating new business ideas
- **Output**: 9-block canvas covering problem, solution, customers, and business model

### SVPG Opportunity Assessment
- **Created by**: Marty Cagan (Silicon Valley Product Group)
- **Purpose**: Evaluate product opportunities
- **When**: Existing products deciding what to build next
- **Output**: 10-question assessment with go/no-go recommendation

### Default: Lean Canvas
The agent uses **Lean Canvas** as default because:
- Most users are validating new ideas (pre-product)
- Covers full business model including revenue/costs
- One-page format is immediately actionable
- Widely recognized and understood

See `/frameworks/comparison.md` for detailed comparison.

## Example Conversation

```
Agent: What problem does your idea solve?

User: We're building a project management tool.

Agent: What specific problem does it solve that existing tools don't?

User: Dev teams can't track dependencies across projects easily.

Agent: ✓ Got it. Problem: tracking cross-project dependencies for dev teams.
Who specifically experiences this?

User: Engineering managers at mid-size tech companies.

Agent: How mid-size? How many engineers? What industry?

User: 50-200 engineers. B2B SaaS companies.

Agent: ✓ Clear. Target: Engineering managers at B2B SaaS companies, 50-200 engineers.
Moving to value proposition.

...

[After completing all skills]

Agent: Your validation canvas is ready: dependency-tracker-validation-canvas.md

**Riskiest Assumption**: Engineering managers will pay $99/month
**Next Step**: Interview 10 engineering managers to validate problem and pricing
```

## Output Example

The agent generates a comprehensive one-pager:

```markdown
# Lean Canvas: Cross-Project Dependency Tracker

## Problem
1. Dev teams lose hours tracking dependencies manually
2. Delays cascade when dependencies aren't visible
3. No single source of truth for cross-project status

## Customer Segments
**Primary**: Engineering Managers at B2B SaaS companies (50-200 engineers)
**Early Adopters**: EMs currently using spreadsheets or Jira add-ons

## Unique Value Proposition
Real-time dependency mapping across all projects without manual updates

## Solution
1. Auto-detect dependencies from Git/Jira
2. Visual dependency graph
3. Automated alerts when blockers arise

...

## Riskiest Assumption
Engineering managers will pay $99/month per team

## Next Steps
1. Interview 10 engineering managers
2. Test pricing with 5 prospects
3. Build basic dependency detection prototype
```

## Implementation

### For AI Platform Developers

See `/agent/implementation-guide.md` for detailed instructions on:
- How to load agent components
- State management
- Skill progression logic
- Output generation
- Platform-specific implementations (Claude, GPT, etc.)

### Core Requirements

Your AI platform needs:
1. **System prompt support** (to load agent instructions)
2. **Conversation history** (to maintain context)
3. **File generation** (to save output)
4. **State persistence** (to track skill progression)

## Customization

### Change Output Format

Edit templates in `/templates/`:
- `lean-canvas-template.md` - Default output
- `opportunity-assessment-template.md` - SVPG format
- `output-onepager-template.md` - Executive summary

### Modify Skills

Edit files in `/agent/skills/` to:
- Add/remove questions
- Change validation criteria
- Adjust behavior for that skill

### Add New Framework

1. Create new template in `/templates/`
2. Document framework in `/frameworks/`
3. Update agent config to support it

## Best Practices

### For Users

1. **Be specific** - Generic answers get challenged
2. **Quantify when possible** - Numbers are better than adjectives
3. **Mark unknowns** - It's OK to say "TBD, need to research"
4. **Test assumptions** - Use the output to run experiments

### For Implementers

1. **Don't let agent hallucinate** - Enforce evidence-based responses
2. **Maintain brevity** - Max 2-3 sentences per response
3. **Challenge vagueness** - Push for specific, actionable answers
4. **Highlight risks** - Focus on what could invalidate the idea

## Contributing

We welcome contributions:

- **Skills**: Improve questions or validation criteria
- **Templates**: Add new output formats
- **Frameworks**: Document additional methodologies
- **Documentation**: Clarify or expand guides

## Resources

### Learn More About Methodologies
- [Lean Canvas](https://leanstack.com) - Official Lean Canvas site
- [SVPG](https://www.svpg.com) - Silicon Valley Product Group articles
- "Running Lean" by Ash Maurya - Book on Lean Canvas
- "Inspired" by Marty Cagan - Book on SVPG product discovery

### Validation Resources
- "The Mom Test" - How to talk to customers
- "Testing Business Ideas" - Validation experiments
- "Lean Startup" - Eric Ries' foundational book
- "Value Proposition Design" - Customer-centric validation

## FAQ

**Q: How long does validation take?**
A: 20-60 minutes for a complete canvas, depending on how prepared you are.

**Q: Can I skip skills?**
A: Yes, though we recommend completing all for comprehensive validation.

**Q: What if I don't know the answer?**
A: Mark it as "TBD - Requires validation" and make it a test priority.

**Q: Can I update my canvas later?**
A: Yes! The canvas is a living document. Update as you learn.

**Q: Do I need to validate everything before building?**
A: No. Validate the riskiest assumptions first, then iterate.

**Q: Is this for B2B or B2C?**
A: Both. The frameworks work for any business model.

## License

[Specify your license]

## Support

- **Documentation**: See `/docs/` folder
- **Issues**: [GitHub Issues](link)
- **Questions**: [Discussion Forum](link)

---

**Ready to validate your idea?** Start by reading `/docs/getting-started.md` then engage with the agent!
