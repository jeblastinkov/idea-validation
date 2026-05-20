# Resco Studio: Feature → Business Value Map

**Date**: 2026-05-19 | **Version**: 1.1 | **Owner**: Resco Product Team
**Purpose**: Map each Studio capability to persona, business problem, revenue impact, and priority — to guide v1/v2/v3 sequencing decisions.

---

## How to Read This Document

Each capability is scored across four dimensions:

| Dimension | What it measures |
|---|---|
| **Business Value Type** | Retention / Acquisition / Upsell / Efficiency |
| **Revenue Impact** | Direct (generates new €) or Indirect (protects or enables €) |
| **Strategic Importance** | H / M / L — how critical to Resco Studio's core promise |
| **Build Complexity** | H / M / L — effort relative to other capabilities (not absolute) |

**Priority score** = Business Value × Strategic Importance ÷ Build Complexity (qualitative).

---

## Summary Matrix

| # | Capability | Persona | Phase | Value Type | Revenue Impact | Strategic | Complexity | Priority |
|---|---|---|---|---|---|---|---|---|
| 1 | AI Project Modifier (App Builder) | App Maker | v1 | Acquisition + Upsell | Direct | **H** | H | **P1** |
| 2 | Home Replacement Builder | App Maker | v1 | Acquisition + Upsell | Direct | **H** | M | **P1** |
| 3 | Notes (Notebook LLM) | App Maker | v1 | Retention + Upsell | Indirect | **H** | M | **P1** |
| 4 | AI Forms / Questionnaire Builder | Field Service Mgr | v1 | Acquisition + Retention | Direct | **H** | M | **P1** |
| 5 | MCP Hub | App Maker | v1 | Acquisition + Upsell | Direct | M | M | **P2** |
| 6a | External Data Collection (non-licensed users) | External parties | v2 early | **Acquisition (new market)** | **Direct** | **H** | M | **P1** ⬆️ |
| 6b | External User Management (admin) | IT Admin | v2 | Retention + Efficiency | Indirect | M | M | **P2** |
| 7 | Sync Log Analyzer | IT Admin / App Maker | v2 | Retention + Efficiency | Indirect | M | L | **P2** |
| 8 | AI Usage Monitoring | IT Admin | v2 | Upsell + Efficiency | Direct | M | L | **P3** |
| 9 | Billing & License Management | IT Admin | v2 | Efficiency + Upsell | Direct | M | M | **P3** |

---

## Capability Detail

---

### 1. AI Project Modifier — App Builder
**Persona**: App Maker (IT Manager)
**Phase**: v1 — working today

**Problem it solves**:
IT Managers spend hours manually configuring Resco apps in Woodford, then context-switching to ChatGPT to generate JavaScript with no Resco awareness — producing generic, often incorrect output they must debug manually.

**What it does**:
Natural language chat that reads the customer's full Resco project (entities, workflows, data model, relationships) and modifies it directly — creating list views, detail forms, custom actions, JavaScript logic, multi-backend connections (Dataverse, Dynamics, ServiceNow, Salesforce).

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Acquisition** | "AI that builds Resco apps by chat" is a headline differentiator vs Salesforce, MS, ServiceNow native tools | High — primary reason a new customer would choose Resco |
| **Upsell** | Primary driver of €100/user/month seat + AI credits consumption | Direct revenue |
| **Retention** | Deep project integration makes switching costly | Medium — stickiness |

**Why it's P1**: It is the product's core promise. Everything else in Resco Studio is supporting capability. Without this working well, the entire platform loses its reason to exist.

**Risk**: AI output quality must be high enough that IT Managers trust it with their live production project on first use. One bad modification that breaks a Resco deployment = loss of trust that is very hard to recover.

**Key metric**: % of users who complete first successful AI-driven project modification within 30 minutes of onboarding.

---

### 2. Home Replacement Builder
**Persona**: App Maker (IT Manager)
**Phase**: v1 — working today

**Problem it solves**:
Custom home screens (home replacements) in Resco are one of the most requested but most time-consuming customizations — currently requiring manual Woodford configuration and JavaScript. Many customers use generic Resco home screens because custom ones take too long to build.

**What it does**:
Dedicated AI-assisted canvas for designing and deploying custom Resco home screens. Includes a reusable UI component library built from real customer patterns — drag-to-compose + AI refinement. Output is a working Resco home replacement, deployable without leaving Studio.

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Acquisition** | "Build a custom field app home screen in 20 minutes" is a concrete, demonstrable promise | High — strong demo moment |
| **Upsell** | AI credits consumed per home replacement build | Direct revenue |
| **Retention** | UI template library becomes proprietary asset that grows in value — customers don't want to leave it | Medium-high |

**Why it's P1**: Home replacement is a use case customers understand immediately and can evaluate in a 30-minute demo. It is the fastest path to a "wow" moment for new and existing customers alike.

**Compounding asset**: Every home replacement built becomes a potential template. The template library is a moat that gets stronger with every customer — no competitor can replicate it without years of Resco customer data.

**Key metric**: Number of home replacements deployed via Studio per month; template library size and reuse rate.

---

### 3. Notes — Notebook LLM
**Persona**: App Maker (IT Manager)
**Phase**: v1 — working today

**Problem it solves**:
IT Managers often inherit Resco projects they didn't build — undocumented workflows, unexplained field logic, cryptic JavaScript. Understanding what a Resco project does and why it works the way it does is a major source of friction when onboarding, debugging, or handing off.

**What it does**:
A persistent notebook LLM that works over the entire Resco project. IT Managers add notes (observations, decisions, questions); the AI surfaces insights, explains existing configurations, suggests optimizations, and answers "why does this work this way?" based on both the project structure and the notes. It is a project knowledge base, not a chat session.

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Retention** | Notes becomes the institutional memory of a Resco deployment — extremely high switching cost once in use | High |
| **Upsell** | AI credits consumed for analysis and insight generation | Direct (moderate) |
| **Acquisition** | Differentiator for enterprise customers with complex, long-lived Resco deployments | Medium |

**Why it's P1**: Notes is a sleeper feature — low demo drama but extremely high retention value. Once an IT Manager has 6 months of notes attached to their project, they will not move to a competing tool. It is the feature most likely to create long-term lock-in without feeling coercive.

**What makes it unique**: Unlike chat (stateless), Notes is persistent and project-scoped. It compounds in value the longer a customer uses it — a rare property in AI tooling.

**Key metric**: % of active users with at least 5 notes added; 30/60/90 day retention for Notes users vs non-Notes users.

---

### 4. AI Forms / Questionnaire Builder
**Persona**: Field Service Manager
**Phase**: v1 — working today

**Problem it solves**:
Field Service Managers own the processes their technicians follow in the field but depend on IT to translate those processes into Resco questionnaires. Every form change — a new inspection question, a conditional field, a scoring rule — requires an IT ticket and a wait. This creates a bottleneck between the people who know what the field needs and the people who can build it.

**What it does**:
Natural language form builder that lets Field Service Managers create, modify, and publish Resco questionnaires and inspection forms without touching Woodford or involving IT. Includes a template library for common field service scenarios (safety inspections, work order completion, asset condition surveys, preventive maintenance checklists).

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Acquisition** | Opens a second buyer within each customer account — Field Service Manager can now be a Studio champion alongside IT Manager | High — expands SAM per account |
| **Retention** | Removes IT bottleneck frustration; Field Service Managers who own their forms don't want to go back | Medium-high |
| **Upsell** | Additional seat (€100/month) for Field Service Manager persona — separate from IT Manager seat | Direct revenue: multiplies seats per account |

**Why it's P1**: This is the only v1 capability with a clear, separate buyer persona — meaning it expands revenue per account, not just per-user. If a company has 1 IT Manager and 2 Field Service Managers all using Studio, that's 3 seats vs 1. It is the fastest path to increasing average revenue per account.

**Key insight**: The "no IT ticket" value proposition is immediately understood by Field Service Managers. It doesn't require a product demo — the pain is obvious and the solution is obvious.

**Key metric**: Forms created per Field Service Manager per month; IT ticket volume reduction for questionnaire changes (proxy for value delivered).

---

### 5. MCP Hub
**Persona**: App Maker (IT Manager)
**Phase**: v1 — working today

**Problem it solves**:
MCP (Model Context Protocol) server setup for Resco tools is currently a technical, manual process with no UI. IT Managers who want to connect AI agents to Resco workflows, or add 3rd party MCPs to individual Resco tools, have no guided path — it requires Resco support or advanced technical knowledge.

**What it does**:
Guided UI for setting up, configuring, and managing MCP servers connected to Resco tools. Allows IT Managers to add 3rd party MCPs per tool, manage connections, and expose Resco data/actions to external AI agent workflows — all without manual configuration or Resco support calls.

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Acquisition** | MCP is a growing standard; "Resco works with any MCP-compatible AI agent" is a forward-looking differentiator | Medium — appeals to technically sophisticated buyers |
| **Upsell** | Enables more AI agent workflows → more AI credits consumed | Direct (AI credits) |
| **Retention** | Once MCP connections are live and production-stable, removing them is disruptive | Medium |

**Why it's P2 (not P1)**: MCP Hub is valuable but appeals to a narrower, more technical segment within the IT Manager persona. It is not the primary reason a customer chooses Studio, but it significantly deepens value for customers who discover it. It is a "power user" feature — important for retention of technical champions, less important for initial adoption.

**Key metric**: Number of active MCP connections per account; AI credit consumption from MCP-connected workflows.

---

### 6. External Users — SPLIT INTO TWO DISTINCT CAPABILITIES

**⚠️ Reassessment note (v1.1)**: "External User Management" was originally framed as a v2 admin feature. This is wrong. It conflates two fundamentally different capabilities with very different business value. They must be separated.

---

### 6a. External Data Collection — Forms for Non-Licensed Users
**Persona**: External parties (citizens, contractors, suppliers, insurance claimants, kiosk users) + the IT Manager / Field Service Manager who configures the form
**Phase**: v2 early — should be pulled forward given strategic importance
**Priority**: P1 ⬆️ (reassessed from P2)

**Problem it solves**:
Organizations using Dynamics 365 / Dataverse need to collect structured data from people who are NOT employees and NOT Resco license holders — contractors submitting daily reports, suppliers updating records, citizens filing service requests, insurance claimants recording incident details, airport kiosk users checking in equipment.

Today there is no good solution for this. The options are:

| Current Option | Why it's broken |
|---|---|
| **Microsoft Power Pages** | Requires setup, licensing cost per visitor, overkill for a simple form — and still requires users to navigate a portal |
| **Microsoft Power Apps (canvas)** | Requires app installation or browser access with per-user licensing — unacceptable for one-time or occasional external users |
| **Custom web forms** | Requires development, hosting, manual Dataverse integration — expensive, slow to build, hard to maintain |
| **Paper / email** | Zero structure, manual data entry into Dynamics afterwards |

**The Microsoft licensing trap**: Microsoft's model requires every user who touches Dynamics data to be a paid license holder — even if that person submits one form per month. Power Pages is the only semi-viable workaround but is expensive, complex to configure, and still requires authenticated sessions for anything non-trivial. For external users filling out a single questionnaire, the Microsoft tax is absurd.

**What Resco Studio offers instead**:
A Field Service Manager or IT Manager builds a questionnaire in Forms Studio (already in v1). That form is published as a shareable link or QR code. An external user opens the link in any browser — no app install, no Resco account, no Microsoft license. They fill out the form. Data is written directly to Dataverse / Dynamics in the correct entity and field structure. The external user never knows or cares that Resco or Dynamics is involved.

**Use cases**:
| Use case | External user | Data destination |
|---|---|---|
| Contractor daily report | Field contractor | Dynamics work orders |
| Supplier onboarding | New supplier | Dataverse supplier entity |
| Insurance claim intake | Policyholder | Dynamics case entity |
| Airport equipment check-in | Ground crew / passenger | Dataverse asset entity |
| Citizen service request | Member of public | Dynamics case / service request |
| Safety incident report | Visitor / contractor on site | Dataverse incident entity |
| Inspection sign-off | Subcontractor | Resco questionnaire entity |

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Acquisition — new market segment** | Attracts organizations that use Dynamics/Dataverse but have no viable external data collection story — this is a new buyer who doesn't need to be a Resco mobile app customer first | **Very High** — opens TAM beyond current 550 customers |
| **Acquisition — competitive wedge vs Microsoft** | "Resco collects from external users without per-user licensing; Microsoft charges you for every contractor" is a concrete, financially quantifiable value prop | **High** — directly attacks Microsoft licensing pain |
| **Upsell** | Each published external form drives AI credits (form generation) + potential seat expansion as more Field Service Managers build forms | Direct revenue |
| **Retention** | Organizations that route external data collection through Resco Studio become deeply integrated — migrating means rebuilding all form-to-Dataverse mappings | **High** — strong switching cost |

**Why this is P1, not P2**:
This is not an admin feature. It is a new product surface that addresses a real, painful, underserved problem for which Microsoft's answer ("buy more licenses") is broadly rejected by customers. The TAM is not 550 Resco customers — it is every organization on Dynamics/Dataverse with external data collection needs. That is a significantly larger market.

The Forms Builder (v1, already built) is the foundation. The external-facing, no-account-required publish-and-collect layer is the incremental addition. Build complexity is Medium — the form engine exists; what's needed is an anonymous/token-based access layer and a direct Dataverse write connector.

**Competitive framing**:
> "Power Pages costs money and requires portal setup. Power Apps requires app installation. Resco Studio lets you publish a form as a QR code — a contractor scans it, fills it in, data lands in Dynamics. No license. No install. No friction."

This is a headline-level differentiator that IT buyers and procurement teams immediately understand and can calculate ROI from (license cost saved × number of external users).

**Key metric**: Number of external form submissions per month per account; number of accounts using external form publication; license cost displacement vs Power Pages equivalent.

---

### 6b. External User Management — Admin Portal
**Persona**: IT Admin
**Phase**: v2
**Priority**: P2 (unchanged)

**Problem it solves**:
Organizations with multiple Resco deployments across business units or geographies have no unified view of who has access to what. License management is handled via Resco support calls or manual spreadsheets.

**What it does**:
Unified view of all users across the organization: org unit assignment, Resco license counts, assign/unassign. Replaces manual Resco support calls for user administration.

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Retention** | Self-service reduces friction; reduces dependency on Resco support | Medium |
| **Efficiency** | Reduces Resco support load for license management | Indirect |
| **Acquisition** | Table stakes for enterprise procurement approval | Medium |

**Why it's P2**: Hygiene. Absence can block enterprise deals; presence doesn't win them. Build before enterprise-scale rollout, not before.

**Key metric**: % of user management actions completed self-service vs via Resco support ticket.

---

### 7. Sync Log Analyzer
**Persona**: IT Admin / App Maker (IT Manager)
**Phase**: v2

**Problem it solves**:
When Resco mobile apps fail to sync — data not updating, conflicts, errors — diagnosing the problem requires reading raw sync logs that are dense, technical, and not human-readable without expertise. IT Managers currently need to involve Resco support or spend hours manually parsing logs.

**What it does**:
Structured sync log viewer with filtering (by device, user, date range, error type), error categorization, and AI-assisted diagnosis ("This failure pattern suggests a connectivity timeout during entity X sync — likely caused by Y"). Replaces raw log files with an actionable diagnostic interface.

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Retention** | Reduces support escalation frustration — one of the top sources of customer dissatisfaction with mobile enterprise software | Medium-high |
| **Efficiency** | Reduces Resco support ticket volume for sync diagnostics | Indirect |

**Why it's P2**: High retention value but relatively low build complexity — it is a good "quick win" for v2 that addresses a real pain point without requiring significant new infrastructure. The AI diagnosis layer is what makes it differentiated vs a raw log viewer.

**Key metric**: Support ticket deflection rate for sync-related issues; time-to-diagnosis for sync failures (before vs after).

---

### 8. AI Usage Monitoring
**Persona**: IT Admin
**Phase**: v2

**Problem it solves**:
Organizations adopting AI tooling face budget unpredictability — AI credit consumption is variable and hard to forecast. IT Admins have no visibility into which users or teams are consuming AI credits, making it impossible to manage costs or plan budgets.

**What it does**:
Dashboard showing AI credit consumption by user, team, and feature (App Builder vs Forms Builder vs Notes vs MCP) over time. Includes budget alerts, consumption trends, and per-user breakdown. Enables IT Admins to allocate, monitor, and cap AI spending.

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Upsell** | Visibility into consumption patterns creates natural conversation for expanding AI credit packages | Direct — enables usage-based upsell |
| **Retention** | Budget predictability reduces "surprise bill" churn — a common AI product failure mode | Medium |
| **Acquisition** | Enterprise procurement requires cost control visibility before approving AI tools | Medium — removes procurement blocker |

**Why it's P3**: Critical for the billing/credits revenue model to scale but not needed until AI credit consumption is significant enough to create budget concern. Build when Studio reaches 50+ active users.

**Key metric**: % of accounts that view usage dashboard monthly; AI credit plan upgrades driven by consumption visibility.

---

### 9. Billing & License Management
**Persona**: IT Admin
**Phase**: v2

**Problem it solves**:
Resco license management currently requires contacting Resco — there is no self-service way to add seats, change license tiers, view invoices, or manage subscription details. This is a friction point for growing organizations and a source of support load for Resco.

**What it does**:
Self-service billing portal: view current license tier and seat count, add/remove seats, upgrade/downgrade plan, view and download invoices, manage payment method. Integrates with Resco's existing licensing backend.

**Business Value**:
| Value Type | Mechanism | Estimated Impact |
|---|---|---|
| **Upsell** | Self-service seat addition removes friction from expansion — customers can grow without waiting for a sales call | Direct — removes expansion bottleneck |
| **Efficiency** | Reduces Resco internal sales/support load for routine license changes | Indirect |
| **Acquisition** | Mid-market and above expects self-service billing as baseline | Medium (table stakes) |

**Why it's P3**: High internal efficiency value but low customer excitement. Necessary infrastructure for scale but not a reason anyone buys Studio. Build when Studio has enough paying customers that license management becomes a recurring support burden.

**Key metric**: % of license changes completed self-service vs via Resco sales/support; time-to-seat-expansion.

---

## Prioritization Summary

### v1: Ship Now (P1) — Core Value Promise
These four capabilities deliver the product's core promise to both primary personas. All are working today.

| Capability | Why Ship First |
|---|---|
| **AI Project Modifier (App Builder)** | Core differentiator — the reason Studio exists |
| **Home Replacement Builder** | Fastest "wow" moment; builds the template library moat |
| **Notes (Notebook LLM)** | Highest retention driver; compounds in value over time |
| **AI Forms / Questionnaire Builder** | Opens second buyer persona; multiplies seats per account |

### v1 Supporting / v2 Early (P1–P2): Strategic Acceleration
| Capability | Why Pull Forward |
|---|---|
| **MCP Hub** | Already built; serves technical champions; drives AI credit consumption |
| **External Data Collection (non-licensed users)** | ⬆️ Reassessed to P1 — opens new market beyond 550 existing customers; direct competitive wedge vs Microsoft licensing; Forms Builder foundation already exists |

### v2: Required for Scale (P2) — Hygiene + Retention
| Capability | Why v2 |
|---|---|
| **External User Management (admin)** | Table stakes for enterprise; needed before large account rollout |
| **Sync Log Analyzer** | High retention value, low complexity — good early v2 win |

### v2+: Revenue Operations (P3) — Monetization Infrastructure
| Capability | Why v2+ |
|---|---|
| **AI Usage Monitoring** | Build when AI credit spend creates budget questions at customer level |
| **Billing & License Management** | Build when license management support load justifies self-service investment |

---

## Business Value by Type — Consolidated View

| Business Value Type | Primary Capabilities | Revenue Mechanism |
|---|---|---|
| **Acquisition — existing Resco market** | App Builder, Home Replacement, Forms Builder | New Resco customers won because Studio exists |
| **Acquisition — new market (non-licensed external data)** | **External Data Collection** | Organizations on Dynamics/Dataverse with external user data collection needs — not current Resco customers; Microsoft licensing pain drives them to Resco |
| **Upsell / Expansion** | App Builder, Home Replacement, Forms Builder, MCP Hub, Usage Monitoring, Billing, External Data Collection | Seat expansion (€100/user) + AI credit consumption + form submission volume |
| **Retention** | Notes, Sync Log Analyzer, External Data Collection, User Management | Churn reduction — stickiness and switching cost |
| **Efficiency** | User Management (admin), Sync Logs, Billing | Resco internal support cost reduction |

**Key insight — v1.1 update**: External Data Collection (6a) is the only capability in this map that simultaneously drives acquisition in a *new* market segment AND creates strong retention through deep Dataverse integration. It expands the TAM beyond Resco's 550 existing customers to any organization on Dynamics/Dataverse that needs to collect data from external parties without paying Microsoft per-user licensing. This is the feature most likely to generate inbound acquisition interest from organizations that have never considered Resco before.

**Original key insight (unchanged)**: v1 capabilities win customers, v2 capabilities keep them — both phases are necessary for a healthy business.

---

## Open Questions to Resolve

1. **Notes depth**: Is Notes in v1 read-only (AI explains the project) or read-write (AI modifies project from Notes context)? The answer significantly changes its value proposition and build complexity.
2. **Forms vs App Builder overlap**: Can the AI Project Modifier already build questionnaires, making the dedicated Forms Builder redundant — or is Forms Builder a genuinely simpler, scoped interface for non-technical users? This must be answered to justify separate experiences.
3. **MCP Hub scope**: Which 3rd party MCPs are supported at launch? A curated list of 5-10 (Slack, Jira, ServiceNow, etc.) is more credible than "any MCP" as a launch claim.
4. **AI credits pricing**: What is the unit (per token, per operation, per session)? This determines whether AI Usage Monitoring is urgent or optional in v2.

---

**Created**: 2026-05-19 | **Next Review**: After 10 customer discovery interviews | **Owner**: Resco Product Team
