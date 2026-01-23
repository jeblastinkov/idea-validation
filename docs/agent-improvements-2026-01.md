# Agent Improvements Summary

**Date**: 2026-01-23
**Purpose**: Enhanced validation agent for stricter validation, research capability, and executive output

---

## Overview

The business idea validation agent has been significantly enhanced to be more strict, helpful, and professional in guiding users through Lean Canvas or SVPG Opportunity Assessment creation.

---

## Key Improvements

### 1. Stricter Validation (CRITICAL)

**Problem**: Previous agent accepted vague answers like "everyone", "better", "small businesses"

**Solution**: 3-strike rule with immediate challenges

**Implementation**:
- **1st vague answer**: "Too vague. What SPECIFIC problem?"
- **2nd vague answer**: "Still generic. Can you describe the last time this problem occurred?"
- **3rd vague answer**: "I need specifics to proceed. Should I research, or can you provide details?"

**Examples of rejected vague answers**:
- ❌ "Everyone" / "Companies" / "Small businesses" → ✅ "10-50 person B2B SaaS companies in Western Europe"
- ❌ "Better/Faster/Cheaper" → ✅ "50% faster deployment (from 2 weeks to 1 week)"
- ❌ "The market is huge" → ✅ "TAM: 15,000 consultants, SAM: 80 from 16 partners"

**Blocking progression**: Agent will NOT advance to next skill until answer meets quality standards

---

### 2. Research Capability (NEW)

**Problem**: Users often don't know critical market data (market size, competitor pricing, industry benchmarks)

**Solution**: Agent can now research using WebSearch when user lacks information

**Workflow**:

```
User: "I don't know the market size."

Agent: "Can you estimate based on target customer count?"

User: "No, I really don't know."

Agent: "Let me research that for you."
[Uses WebSearch]

Agent: "I found the global project management software market is $6B
(2024, Gartner). Your segment (dependency tracking) is estimated at
$500M-1B. Does this match your understanding?"

User: "Yes, let's use $800M."

Agent: "✓ Using $800M TAM. Moving on."
```

**What agent can research**:
- ✅ Market sizes (TAM/SAM/SOM)
- ✅ Competitor landscape and pricing
- ✅ Industry benchmarks and trends
- ✅ Technology adoption rates
- ✅ Customer segment demographics

**What agent will NOT research**:
- ❌ User's specific problem (they must know)
- ❌ Their unique value proposition (they define)
- ❌ Their solution approach (their expertise)
- ❌ Internal company capabilities (company-specific)

**Data quality standards**:
- Recent sources (2024-2026)
- Multiple sources if data varies (present range)
- Authoritative sources (industry reports, government data, research firms)
- Always cite: "(Source: Gartner 2024 via WebSearch)"

---

### 3. Executive Output Formatting (ENHANCED)

**Problem**: Previous outputs were verbose (450 lines) and not executive-ready

**Solution**: Strict length targets with professional formatting

**Standards**:
- **Lean Canvas**: 150-200 lines maximum (executive version)
- **SVPG Assessment**: 250-300 lines maximum (executive version)
- **Executive summary** at top (5-line overview: decision, risks, next action)
- **Scannable structure**: Bullets, short paragraphs (max 4 lines)
- **No duplication**: Each point stated once
- **Professional tone**: No emojis (unless explicitly requested)
- **Concise sections**: 10-30 lines per major section
- **Clear hierarchy**: Headers → sub-headers → bullets

**Quality checklist before generation**:
- [ ] All skills completed
- [ ] No vague statements remain
- [ ] Quantified where possible
- [ ] Assumptions marked as "TBD"
- [ ] Researched data cited
- [ ] User confirmed summary
- [ ] Length within target

---

### 4. Zero Hallucination Policy (ENFORCED)

**Rule**: Agent will ONLY use:
1. Information user explicitly provided
2. Information researched via WebSearch and confirmed by user
3. Template structure from Lean Canvas / SVPG frameworks

**Prohibited**:
- ❌ Inventing market sizes
- ❌ Assuming competitor details
- ❌ Creating features user didn't mention
- ❌ Guessing customer pain points
- ❌ Fabricating data or statistics
- ❌ Adding business advice user didn't ask for

**If unsure**: Mark as "TBD - Requires validation" instead of guessing

---

### 5. Professional Tone (STRICT)

**Removed**:
- ❌ "That's a great idea!"
- ❌ "Wow, this is going to be amazing!"
- ❌ "Exciting opportunity!"
- ❌ Generic business advice or lecturing

**Adopted**:
- ✅ "That's a critical assumption. How will you test it?"
- ✅ "This risk could invalidate the idea. Test it first."
- ✅ "✓ Got it. [Brief confirmation]. Moving to [next topic]."

---

## Updated Files

### Core Agent Configuration
1. **system-prompt.md**: Added research capability, stricter validation, executive formatting standards
2. **behavior-guidelines.md**: Added research workflow, 3-strike rule, professional tone requirements

### Skills
1. **01-problem-definition.md**: Enhanced with strictness rules and research examples
2. **09-generate-output.md**: Updated with executive formatting checklist and quality standards

### Templates (Already Optimized)
1. **lean-canvas-template.md**: 150-200 line target with executive summary
2. **opportunity-assessment-template.md**: 250-300 line target with executive summary

---

## Agent Behavior Examples

### Before vs After

#### Example 1: Vague Customer Segment

**Before**:
```
User: "Our target market is small businesses."
Agent: "Great! Moving to value proposition."
```

**After**:
```
User: "Our target market is small businesses."
Agent: "Too broad. Which specific type? How many employees? What industry?"

User: "Tech companies."
Agent: "Still vague. How many employees? B2B or B2C? What geography?"

User: "B2B SaaS, 50-200 employees, Western Europe."
Agent: "✓ Clear. Target: B2B SaaS companies, 50-200 employees, Western Europe. Moving to value proposition."
```

---

#### Example 2: Unknown Market Size

**Before**:
```
User: "I don't know the market size."
Agent: "Mark it as TBD. Moving on."
```

**After**:
```
User: "I don't know the market size."
Agent: "Can you estimate based on target customer count?"

User: "No, I really have no idea."
Agent: "Let me research that for you."
[WebSearch]

Agent: "I found the market for [your segment] is estimated at $500M-1B globally
(Source: Gartner 2024). Your addressable portion is likely 10-20% = $50-200M.
Does this match your understanding?"

User: "Let's use $100M."
Agent: "✓ Using $100M SAM (Source: Gartner 2024 via WebSearch, user-adjusted). Moving on."
```

---

#### Example 3: Generic Problem Statement

**Before**:
```
User: "We make project management easier."
Agent: "What makes you different from competitors?"
```

**After**:
```
User: "We make project management easier."
Agent: "Too generic. What SPECIFIC problem?"

User: "Teams waste time in meetings."
Agent: "How much time? What type of meetings? What specifically goes wrong?"

User: "Dev teams spend 5 hours/week in status meetings because they can't track cross-project dependencies."
Agent: "✓ Got it. Problem: Dev teams lose 5 hours/week tracking cross-project dependencies. Who specifically experiences this?"
```

---

## Expected Outcomes

### User Experience
- **More challenging**: Users will be pushed to think deeply about their idea
- **More helpful**: Agent can research data users don't have
- **Higher quality output**: Professional, executive-ready validation canvas
- **Clear next steps**: Specific action items with timeframes

### Output Quality
- **Concise**: 150-200 lines (Lean) or 250-300 lines (SVPG) vs previous 450+
- **Scannable**: Executives can review in 5-10 minutes
- **Evidence-based**: All data either user-provided or researched + cited
- **Actionable**: Clear risks, assumptions, and next validation steps

### Validation Rigor
- **No vague answers accepted**: 3-strike rule enforces specificity
- **Quantified**: Numbers, percentages, timeframes wherever possible
- **Evidence-backed**: Research capability fills knowledge gaps
- **Honest**: Assumptions marked clearly, risks identified, no cheerleading

---

## Usage Guidelines for Users

### What Changed
1. **Agent is stricter**: You'll be challenged on vague answers—this is intentional
2. **Agent can research**: Say "I don't know" and agent will find data for you
3. **Shorter output**: 150-300 lines instead of 400+, more executive-friendly
4. **Professional tone**: No congratulations, just focused validation work

### How to Get Best Results
1. **Be specific**: Instead of "small businesses", say "10-50 employee SaaS companies in US"
2. **Quantify**: Instead of "faster", say "50% faster (2 weeks to 1 week)"
3. **Say "I don't know"**: Agent will research market data, competitor info, etc.
4. **Confirm research**: Review researched data and adjust if needed
5. **Accept challenges**: If agent pushes back 3 times, your answer IS too vague

### What to Expect
- **10-15 questions** across 8 skills (Lean) or 10 questions (SVPG)
- **20-40 minutes** total conversation time
- **2-5 research queries** if you lack market data
- **150-300 line output** in professional, executive format
- **Clear next action** for immediate validation testing

---

## Technical Implementation

### Tools Used
- **WebSearch**: For market research when user lacks data
- **Read/Write**: For template loading and output generation
- **Validation logic**: 3-strike rule for vague answers

### Data Flow
```
User Input
  ↓
Strictness Check (3-strike rule)
  ↓
Research if Needed (WebSearch + confirmation)
  ↓
Skill Completion Validation
  ↓
Progress to Next Skill
  ↓
Final Summary (user confirmation)
  ↓
Generate Output (executive format, 150-300 lines)
  ↓
Save Markdown File
```

### Quality Gates
1. **Per question**: Answer must be specific, concrete, quantified
2. **Per skill**: All required info collected before advancing
3. **Pre-generation**: User confirms summary, all 8/10 areas complete
4. **Post-generation**: Output within length target, professional format

---

## Migration Notes

### Backwards Compatibility
- Existing templates work with new agent (already optimized for 150-300 lines)
- Previous verbose outputs (450+ lines) still accessible as comprehensive versions
- No breaking changes to conversation flow

### Recommended Action
- Users should re-run validations using enhanced agent for executive-ready output
- Compare v1 (comprehensive 450 lines) with v2 (executive 150-300 lines)
- Use v2 for stakeholder presentations, v1 for deep-dive reference

---

## Success Metrics

### Agent Performance
- **Vague answer rejection rate**: Target >80% (previously ~20%)
- **Research queries per session**: Expected 2-5 (previously 0)
- **Output length**: 150-300 lines (previously 450+)
- **User confirmation required**: 100% (previously optional)

### Output Quality
- **Executive readiness**: Can be presented to C-level without editing
- **Scannability**: 5-10 minute read time (previously 15-20 min)
- **Actionability**: Specific next steps with timeframes
- **Accuracy**: Zero hallucinated data (all user-provided or researched + cited)

---

## Future Enhancements

### Potential Additions
1. **Industry-specific templates**: SaaS, eCommerce, Marketplace, B2B, etc.
2. **Validation experiment library**: Pre-built test plans for common assumptions
3. **Competitive intelligence**: Automatic competitor research and analysis
4. **Financial modeling**: Integrated unit economics calculator
5. **Risk scoring**: Quantitative risk assessment based on market data

### Under Consideration
- Multi-language support (currently English only)
- Integration with market research databases (Gartner, Forrester)
- Collaborative validation (multiple stakeholders)
- Version control and change tracking

---

**Summary**: The enhanced agent is significantly stricter, more helpful (research), and produces professional, executive-ready outputs. Users will experience more rigorous validation but receive higher-quality, actionable results.
