# Lean Canvas: Resco Studio

**Date**: 2026-05-19 | **Version**: 1.1 | **Status**: Initial Validation

---

## Executive Summary

**Idea**: Resco Studio is a paid cloud platform that gives Resco enterprise customers a unified interface to build, configure, and manage Resco mobile applications using Resco-native AI — replacing fragmented tools and manual Resco support with self-service.

**Target**: 550 existing Resco enterprise customers (550–2,200 IT Managers) + new customer acquisition driver globally.

**Economics**: €100/user/month + AI credits consumption | 20 paying users by end of 2026 = ~€24K ARR seats + credits.

**Risk**: Enterprise security/compliance teams block access to a 3rd party cloud tool that connects to Dynamics/Salesforce/ServiceNow environments.

**Next Action**: Run 10 discovery calls with IT Managers at existing Resco customers to validate willingness to pay €100/month and identify top compliance blockers.

---

## Problem

### Top 3 Problems
1. **Fragmented tooling** — IT Managers juggle Resco App Configurator (Woodford), Questionnaire Designer, and external AI tools separately with no unified context.
2. **No self-service for new capabilities** — customers had to contact Resco via call/email to access new services; no automated path existed.
3. **Generic AI has no Resco context** — using ChatGPT/Copilot with Woodford works but produces generic output; no tool understands the customer's specific Resco project structure, data model, or workflows.

### Existing Alternatives
- **Resco App Configurator (Woodford)** — app configuration, no AI, desktop-heavy
- **Resco Questionnaire Designer** — standalone form builder, no integration with app config
- **ChatGPT / GitHub Copilot** — generic JavaScript generation, no Resco project awareness, requires manual context injection every session

---

## Customer Segments

**Primary — App Maker (IT Manager)**: IT Managers at Resco enterprise customers — build and configure Resco mobile apps, manage field service logic, maintain integrations with Dynamics/Salesforce/ServiceNow. Uses Vibe Studio, MCP Hub, Notes.

**Secondary — Field Service Manager**: Operations/Field Service Managers — responsible for field worker processes, create dynamic forms and questionnaires for technicians. Uses AI Forms Builder. (Active in v1, primary focus in v2.)

**Tertiary — IT Admin**: IT/System Administrators — manage organizational access, licenses, billing, compliance. Uses Admin Portal. (v2.)

**Market size**: 550 enterprise customers × 1–4 IT Managers = **550–2,200 direct users** (installed base). Broader TAM: enterprise field service management software market — TBD, requires research.

**Reachability**: Direct through Resco CSM/account management team | Resco partner network | Resco community and documentation channels.

---

## Persona Experiences

Resco Studio is one platform with **three distinct experiences** — each persona lands in a tailored workspace:

### Experience 1: App Maker (IT Manager)
**Entry**: Vibe Studio workspace
- **App Builder** — AI chat that reads the full Resco project (data model, workflows, entities) and builds or modifies mobile app components via natural language. Produces working home replacements, list views, detail forms, custom actions.
- **Home Replacement** — dedicated AI-assisted canvas for designing and deploying custom Resco home screens; reusable UI component library built on real customer patterns.
- **MCP Hub** — setup, configure, and manage MCP servers connected to Resco tools; add 3rd party MCPs per tool.
- **Notes** — Notebook LLM that works across the entire project; surfaces insights, suggests optimizations, answers "why does this workflow work this way?" questions based on project context.

### Experience 2: Field Service Manager
**Entry**: Forms Studio workspace
- **AI Questionnaire Builder** — create, modify, and publish Resco questionnaires and inspection forms via natural language. No Questionnaire Designer needed.
- **Template Library** — pre-built questionnaire templates for common field service scenarios (safety inspections, work order completion, asset surveys); editable via AI.
- Scoped view: no access to code/app config, no Vibe Studio — simplified, role-appropriate UI.

### Experience 3: IT Admin *(v2)*
**Entry**: Admin Portal workspace
- **External User Management** — view all users across the organization, assign/unassign Resco licenses, manage access by org unit.
- **Sync Log Analyzer** — diagnose mobile app sync failures; filter by device, user, date, error type.
- **AI Usage Monitoring** — track AI credit consumption per user and team.
- **Billing & Licensing** — manage Resco license tiers, view invoices, adjust seat counts.

---

## Unique Value Proposition

**"We help Resco IT Managers build and modify Resco mobile apps in minutes — by chatting in natural language with an AI that fully understands their project."**

**High-level concept**: GitHub Copilot, but purpose-built for Resco — knows your data model, your workflows, your UI components, your backends.

**Why different**:
- vs Woodford: AI-native, natural language interface, cloud-based, no manual config
- vs ChatGPT+Woodford: OOTB Resco context, no manual prompt engineering, reusable UI templates, modifies project directly
- vs Salesforce/MS native AI builders: Resco-specific, works across multi-backend (Dataverse, Dynamics, ServiceNow, Salesforce)

---

## Solution

### v1 Features (All Working Today)
1. **AI Project Modifier (Vibe Studio)** — natural language chat that reads and modifies the customer's Resco project: home replacements, UI components, workflows, JavaScript logic
2. **MCP Server Setup** — configure and connect MCP servers to Resco tools; add 3rd party MCPs
3. **AI Forms / Questionnaire Builder** — create and modify Resco questionnaires via AI, replacing Questionnaire Designer

### Delivery Channel
Web-based cloud platform (SaaS).

### NOT in v1 (Deferred to v2)
- External user management (org assignment, license counts)
- Sync log analyzer (mobile app diagnostics)
- AI usage monitoring dashboard
- Billing & license management

---

## Unfair Advantage

**Resco owns the project schema and data model** — no third party can build Resco-native AI with the same depth of context. Resco Studio has direct API access to the customer's Resco project that no external tool can replicate without significant integration effort.

Reusable UI template library built on real Resco customer patterns — grows as a proprietary asset over time.

---

## Channels

**Primary**: Resco CSM and account management team — direct outreach to existing 550 customers.

**Early adopters**: Identify 10–20 power users from existing customer base (IT Managers already experimenting with AI tools for Resco customization).

**Community/Content**: Resco developer documentation, Resco Community portal, YouTube tutorials on Vibe Studio.

**Launch strategy**: 
1. Closed beta with 10 existing customers → gather feedback
2. General availability to existing 550 customers
3. Use as acquisition driver in Resco sales motion for new logos

---

## Economics

**Revenue model**: Hybrid — €100/user/month seat license + AI credits consumption (variable).

**Per-customer revenue**: 2 IT Managers × €100/month × 12 months = **€2,400/year per customer** (seats only) + AI credit consumption on top.

**Investment**: TBD — core product already built; primary costs are infrastructure (cloud IDE containers), AI model costs, and GTM.

**2026 Forecast**:
- 20 paying users × €100/month = **€2,000 MRR / €24,000 ARR** (seats)
- AI credits: TBD — requires usage data
- Conservative Year 1: €24K–€50K ARR depending on AI credit consumption

**Break-even**: TBD — requires infrastructure cost baseline.

---

## Key Metrics

**North Star**: Monthly Active Users building/modifying Resco projects via AI.

**2026 Targets**:
- End of 2026: 50 active users (free + paid)
- End of 2026: 20 paying users
- End of 2026: €24K ARR minimum (seats)

**Supporting metrics**:
- Activation rate: % of trialing IT Managers who complete first AI project modification
- Retention: % of paying users active month-over-month
- AI credits consumed per user/month (signals engagement depth)
- Net new Resco customers citing Studio as purchase driver (acquisition metric)

---

## Critical Risks

**Riskiest assumption**: Enterprise IT/security teams will approve Resco Studio as a cloud tool connecting to their Dynamics/Salesforce/ServiceNow environment — this is unvalidated and is the #1 adoption blocker.

### Top Risks

1. **Security/Compliance Block (CRITICAL)**: Enterprise IT policies block 3rd party cloud tools from accessing production CRM/ERP environments → kills adoption before it starts.
   - *Mitigation*: SOC2 certification, SSO/SAML support, data residency options, on-prem/private cloud deployment option; proactively document security architecture for IT approval processes.

2. **Willingness to Pay (HIGH)**: IT Managers or their budget owners resist €100/month when ChatGPT+Woodford is a free-ish workaround → low conversion from free trial to paid.
   - *Mitigation*: Demonstrate clear time savings with concrete before/after comparison (e.g., "2 hours → 10 minutes for UI component build"); offer reusable template library as tangible proof of value.

3. **Adoption Inertia (HIGH)**: IT Managers are habituated to Woodford; changing workflow requires retraining and organizational buy-in → slow ramp even among willing customers.
   - *Mitigation*: Seamless Woodford import, familiar concepts, short onboarding path (<30 min to first value), champion program with early adopters.

4. **AI Output Quality (MEDIUM)**: AI modifies Resco projects incorrectly or produces buggy JavaScript → erodes trust, users revert to manual.
   - *Mitigation*: Preview/diff before apply, rollback capability, human-in-the-loop confirmation for destructive changes.

5. **Pricing vs Existing AI Spend (MEDIUM)**: Organizations already paying for Microsoft Copilot or enterprise ChatGPT resist additional AI cost → budget fatigue.
   - *Mitigation*: Position as Resco-specific productivity tool (replaces Woodford time, not generic AI); quantify ROI in field service hours saved.

**Key unknowns**:
- Actual compliance approval process duration at target enterprises
- Average AI credit consumption per active user/month
- Conversion rate: trial → paid at €100/month price point
- Whether Field Service Managers (v2 persona) are a faster path to adoption than IT Managers

---

## Next Steps

**THIS MONTH: Validate willingness to pay and compliance blocker with 10 existing Resco customers.**

**Setup**: CSM team identifies 10 IT Managers from existing 550 customers who are currently using external AI tools for Resco customization. 30-minute structured interview: show live Vibe Studio demo, present €100/month pricing, ask about compliance approval process.

**Measure**:
- "Would you pay €100/month for this?" → target 6/10 yes or strong interest
- "Would your IT security team approve this tool?" → identify blockers
- "How long would approval take?" → estimate GTM timeline

**Decision criteria**:
- ✅ 6+/10 interested + compliance path exists → proceed to closed beta
- ⚠️ 4–5/10 interested OR compliance major blocker → adjust pricing or build security package first
- ❌ <4/10 interested OR compliance universally blocks → re-evaluate positioning and pricing

**Timeline**:
- May–June 2026: 10 customer discovery interviews
- July 2026: Closed beta with 5 willing customers
- September 2026: GA launch to existing 550 customers
- Q4 2026: First 20 paying users target

---

## Key Assumptions

1. IT Managers will pay €100/month for Resco-native AI vs free alternative (ChatGPT+Woodford)
2. Enterprise security teams will approve a 3rd party cloud tool with access to Dynamics/Salesforce
3. Resco-native AI context produces meaningfully better output than generic AI + manual prompting
4. 50 active users is achievable from 550-customer base by end of 2026
5. AI credits consumption will generate meaningful revenue above seat licenses
6. Reusable UI template library is a compelling differentiator vs generic AI
7. Vibe Studio (AI project modifier) is the primary driver of adoption — not forms builder or MCP
8. Field Service Managers (forms persona) will be addressed adequately in v2 timing

---

## Reality Check

Resco Studio's core product is built and differentiated — the Resco-native AI context is a genuine moat that no external tool replicates. The primary risk is not product quality but enterprise procurement: security approval timelines at large enterprises can take 3–12 months, which compresses the 2026 timeline significantly if not addressed proactively.

The €100/month price point needs validation — it is high relative to generic AI tools but low relative to enterprise productivity software; the outcome-based value story (hours saved on Resco app builds) must be quantified to justify it.

**Success depends on**:
1. At least one clear compliance approval pathway documented (SOC2 or equivalent)
2. Demo that converts skeptical IT Managers in under 30 minutes
3. CSM team actively selling/introducing Studio to existing 550 customers
4. AI output quality high enough that first-time users trust it with their live project

**If compliance blocks adoption**: Build a sandboxed/demo environment path that lets IT Managers trial with synthetic data, reducing security approval barrier for initial evaluation.

**Remember**: The 2026 target of 20 paying users is conservative — the real prize is making Studio the reason new enterprises choose Resco over Salesforce Field Service or Dynamics FSM.

---

**Created**: 2026-05-19 | **Next Review**: 2026-06-16 | **Owner**: Resco Product Team
