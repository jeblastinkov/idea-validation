# Resco Studio — Executive Briefing

**Date**: 2026-05-21 | **Audience**: CEO, Head of Product, CTO | **Status**: Investment Decision Requested
**Decision sought**: Approve closed beta launch (July 2026) and GA timeline (September 2026)

---

## TL;DR

- **What**: A paid cloud platform that lets Resco customers build, configure, and run Resco deployments via natural language — across Vibe Studio (App Maker), Forms Studio (Field Service Manager), and Admin Portal (IT Admin).
- **Foundation**: Resco Studio runs on top of the customer's existing Dataverse, Dynamics 365, Salesforce, or ServiceNow backend. No standalone database, no migration — it layers AI and tooling on what customers already own.
- **Why invest**: Core product is already built. Competitors (Microsoft, Salesforce, ServiceNow) shipped AI app builders in 2025–2026; the window to own *AI-native Resco development* is open now and closing.
- **Return**: An IT Manager saves ~€16,500/year in reclaimed hours — their Studio seat costs €1,200/year. **Studio pays for itself 13× over in Year 1 on time savings alone.**
- **Risk**: Two unknowns — enterprise compliance approval pathway and willingness-to-pay at €100/seat. Both are testable in a 4-week discovery sprint before GA.
- **Ask**: Approve discovery sprint + closed beta + September GA launch.

---

## What Resco Studio Is

A unified cloud workspace that replaces today's fragmented Resco tooling — Woodford, Questionnaire Designer, and external AI tools — with a single AI-native platform where the AI already understands the customer's exact Resco project.

> **One platform. Three experiences. Resco-native AI that knows your project before you type the first word.**

### Built on what customers already own

Resco Studio is not a standalone product. It connects to the customer's existing backend — Dataverse, Dynamics 365, Salesforce, or ServiceNow — and reads their live Resco project. The AI understands entities, workflows, data relationships, and existing configurations. It modifies the actual project directly. No export, no import, no parallel environment to maintain.

---

## The Problem

Resco customers manage their deployments across four disconnected places: Woodford for app config, Questionnaire Designer for forms, ChatGPT for JavaScript (with no Resco context), and Resco support tickets for everything else. Nobody has the full picture. Every change takes longer than it should.

Specifically:
- **IT Managers** waste 1–2 hours per day switching between Woodford and ChatGPT — and ChatGPT hallucinates because it has no Resco project context.
- **Field Service Managers** depend on IT for every form change — creating a queue between people who know what the field needs and people who can build it.
- **External data collection** (contractors, suppliers, claimants, citizens) has no good answer — Power Pages is overkill, Power Apps requires licensing every user, paper/email is unstructured.
- **New capabilities** Resco wants to offer (MCP, Vibe Studio, home replacements, AI agent workflows) have no self-service path — they generate support tickets, not revenue.

---

## The Solution

Three role-specific experiences in one platform:

| Persona | Workspace | What changes for them |
|---|---|---|
| **App Maker (IT Manager)** | **Vibe Studio** — AI App Builder, Home Replacement Builder, MCP Hub, Notes (Notebook LLM) | Build and modify Resco apps in natural language; AI knows the entire project |
| **Field Service Manager** | **Forms Studio** — AI Questionnaire Builder + template library | Create and publish forms without IT tickets; publish externally as QR/link for non-licensed users |
| **IT Admin** *(v2)* | **Admin Portal** — user mgmt, license mgmt, sync log analyzer, AI usage monitoring | Self-serve everything currently requiring a Resco support call |

---

## What Ships in v1 — MVP Feature List

All five capabilities are working today. Investment required is operational hardening (security, scale, GTM enablement), not product engineering.

| # | Capability | Who uses it | What it does |
|---|---|---|---|
| 1 | **AI Project Modifier** | IT Manager | Chat with AI in natural language — it reads the live Resco project and modifies list views, forms, workflows, and JavaScript directly. No Woodford manual config. |
| 2 | **Home Replacement Builder** | IT Manager | AI-assisted canvas for custom Resco home screens with a reusable UI template library. Hours of manual work → minutes. |
| 3 | **Notes (Notebook LLM)** | IT Manager | Persistent knowledge base for the Resco project. Explains existing configuration, answers "why does this work this way?", and suggests improvements. Compounds in value over time. |
| 4 | **AI Forms / Questionnaire Builder** | Field Service Manager | Build, modify, and publish Resco questionnaires by describing what you need. Forms can be shared as QR code or link — accessible to external users (contractors, suppliers, citizens) without a Resco license. |
| 5 | **MCP Hub** | IT Manager | Configure Resco as an MCP server and connect third-party MCP tools — enabling AI agent workflows that reach into and out of the Resco project. |

**Deferred to v2**: Admin Portal (user management, billing, sync log analyzer, AI usage monitoring), volume-tiered external user pricing.

---

## Onboarding — How a New User Gets Started

### If you already have a Resco project
Connect Studio to your existing Dataverse / Dynamics 365 / Salesforce / ServiceNow backend. Studio reads your live project automatically. No setup, no import — you're in the AI assistant within minutes.

### If you don't have a Resco project yet
Resco hosts a **demo backend** on Resco cloud — a pre-configured Resco project with real data, real entities, and real workflows. New users try Studio against this demo environment immediately, with no backend account or IT approval required.

This removes the single biggest onboarding barrier: *"I need to get IT to give me access to our Resco project before I can evaluate this."*

Demo → connect your real project → start paying. The onboarding path is self-serve from day one.

**Target**: New user completes first AI-driven project modification within 30 minutes of signup.

---

## Value Proposition

**For Resco customers**: The only AI development environment that understands your Resco project — its data model, workflows, entities, and integrations — and modifies it directly through natural language.

**Against competitors**: Microsoft Power Apps Vibe is MS-only. Salesforce MAGE is a developer-only scaffolder. ServiceNow Build Agent has no offline. Resco Studio is the only AI builder that works across Dynamics, Salesforce, ServiceNow, and Dataverse — with no compilation, no app store, no Xcode.

---

## ROI — How the Money Works

### The simple version

A typical IT Manager at a German enterprise costs ~€50/hour (salary + employer overhead). They currently spend **1.5 hours per day** on Resco configuration tasks that Studio automates or accelerates.

**That's €16,500 saved per IT Manager per year.**

A Studio seat costs **€1,200/year** (€100/month).

**Studio pays for itself 13× over in Year 1. Payback in under 1 month.**

---

### All three personas — Year 1 savings

| Role | Time saved | Hourly cost | Annual saving |
|---|---|---|---|
| IT Manager (1 seat) | 1.5 hrs/day | €50/hr | **€16,500** |
| Field Service Manager (2 seats) | 0.5 hrs/day each | €40/hr | **€8,800** |
| **Total time savings** | | | **€25,300** |

**Total Studio cost** (3 seats + AI credits): €4,200/year

**Net saving**: €21,100 | **ROI: 502%** | **Payback: 2 months**

---

### Scenarios

| Scenario | Seats | Studio Cost/yr | Value Delivered/yr | ROI | Payback |
|---|---|---|---|---|---|
| **Minimum** — 1 IT Manager | 1 seat | €1,800 | €16,500 | **817%** | < 2 months |
| **Base** — 1 IT + 2 FS, 300 ext. users | 3 seats | €15,000 | ~€21,160 | **41%** | 8.5 months |
| **Growth** — 2 IT + 3 FS, 1,000 ext. users | 5 seats | ~€38,000 | ~€38,760 | **2%** ⚠️ | ~12 months |

> **Note on external users**: At €3/user/month, Resco is competitive vs Microsoft pay-as-you-go (€3.70) at all volumes but is more expensive than Microsoft annual plan above ~62 users/month. **The seat ROI stands regardless.** Volume-tiered external user pricing is flagged for v2 to address high-scale accounts.

---

### Why the time savings are real

IT Managers report using ChatGPT to generate Resco JavaScript, then spending equal time debugging because ChatGPT has no Resco context. Studio eliminates that loop entirely — the AI knows the project data model, so generated code works first time. One correct modification replaces 2+ hours of manual configure → test → debug → repeat.

---

## Business Case

### Revenue Model
- **Seat license**: €100/user/month (IT Manager + Field Service Manager)
- **AI credits**: consumption-based (per token/operation — TBD)
- **External user fee**: €3/external user/month for forms exposed to non-licensed users

### Market
- **Installed base**: 550 enterprise Resco customers
- **Addressable seats**: 1,100–3,850 (1–4 IT Managers + 1–3 FS Managers per account)
- **New-logo TAM**: Any organization on Dynamics/Dataverse needing external data collection — materially larger than 550

### 2026 Targets
- **50 active users**, **20 paying** = **€24K ARR** (seats) + AI credits
- Closed beta: July | GA: September | First 20 paying: December

---

## Strategic Rationale — Why Resco Should Invest

1. **The product is already built.** Core capability (AI Project Modifier, Forms Builder, MCP Hub) is working today. Investment is operational (security certs, GTM, infrastructure), not engineering.

2. **The window is open now.** Microsoft Power Apps Vibe, Salesforce MAGE, and ServiceNow Build Agent all shipped in 2025–2026. Customers are forming habits around AI development tools right now. Resco must be in their consideration set this year — not next.

3. **Resco's moat is unique and undefendable by competitors.** No external AI can match Resco-native project context. No competitor's AI builder works across Dynamics + Salesforce + ServiceNow. No competitor has 18 years of offline-first mobile container production data. These advantages compound; competitors cannot copy them quickly.

4. **Acquisition driver beyond the 550 base.** External Data Collection opens a new market segment — organizations on Dynamics/Dataverse with external user pain. They never needed to be Resco mobile customers to buy this.

5. **Switching cost engine.** Notes (Notebook LLM) and the UI template library compound in customer value over time. A customer with 12 months of project notes in Studio is functionally locked in — without coercion.

---

## Risks & Mitigations

| Risk | Level | Mitigation |
|---|---|---|
| Enterprise security/compliance blocks 3rd party cloud tool | **High** | SOC2 in progress; SSO/SAML in v1; sandboxed trial environment for evaluation |
| Willingness-to-pay €100/seat unvalidated | Medium | 10 discovery interviews before GA — confirms or adjusts before commitment |
| €3 external user fee uncompetitive vs MS annual at scale | Medium | Volume-tiered pricing in v2; lead with time savings, not licensing savings |
| AI output quality erodes trust on first use | Medium | Preview/diff before apply; rollback on every modification; AI must explain *what* it will change before changing it |
| CSM bandwidth to introduce Studio to 550 accounts | Low–Medium | Phased rollout; CSM enablement playbook; demo automation |

**Biggest unknown**: enterprise compliance approval timeline. **Test plan**: 10 structured customer interviews in May–June 2026 to characterize the approval process before GA commitment.

---

## What Resco Spends vs What Resco Gets

### Year 1 Investment (estimated; full cost baseline TBD)
- SOC2 certification process
- Cloud infrastructure (multi-tenant container IDE + AI model API costs)
- CSM enablement + sales materials
- 1–2 product/engineering FTE for hardening and v2 capabilities

### Year 1 Return
- €24K ARR (conservative seat revenue) + AI credits + external user fees
- New-logo acquisition attribution (TBD as deals close)
- Reduced support load on Resco team for tasks now self-service
- Competitive defense: customers don't migrate to MS/Salesforce because Resco now has AI

### Break-even
Estimated 30–50 paying users at €100/month + AI credits. **Achievable from existing 550-customer base with modest CSM effort.**

---

## Decision Required

✅ **Approve**:
1. Discovery sprint — 10 customer interviews, May–June 2026
2. Closed beta — 5–10 customers, July 2026
3. GA launch to existing 550 customers — September 2026
4. v2 roadmap: Admin Portal + volume-tiered external user pricing — Q1 2027

⚠️ **Conditional gates**:
- After discovery sprint (end of June): proceed to closed beta only if 6+/10 customers confirm WTP and compliance pathway is <90 days
- After closed beta (end of August): proceed to GA only if onboarding-to-first-value is <30 minutes for 7+/10 beta users

❌ **Pause if**:
- Discovery shows universal compliance block → pivot to sandboxed "Studio Lite" tier first
- Discovery shows <4/10 WTP → revisit pricing and v1 positioning before GA

---

## Supporting Documents

For deeper detail, see:
- `resco-studio-validation-canvas-v1.md` — full Lean Canvas
- `resco-studio-svpg-opportunity-assessment-v1.md` — investment case with risk analysis
- `resco-studio-feature-business-value-map.md` — feature prioritization
- `resco-studio-roi-calculator.md` + `.html` — account-level ROI scenarios
- `resco-studio-product-brief-v1.md` — customer-facing narrative

---

*Prepared: 2026-05-21 | Owner: Resco Product Team | Next review: After discovery sprint (end of June 2026)*
