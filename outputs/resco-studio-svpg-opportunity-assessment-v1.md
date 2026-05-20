# Opportunity Assessment: Resco Studio

**Date**: 2026-05-19 | **Product**: Resco Studio | **Team**: Resco Product Development

**Decision**: ✅ **PURSUE** — core product built, differentiation validated, window open now | **Biggest Risk**: Enterprise security/compliance adoption barrier (High)

---

## Executive Summary

**Opportunity**: Paid cloud platform giving Resco enterprise customers a unified, AI-native workspace to build, configure, and manage Resco deployments — replacing fragmented tooling and manual Resco support with three role-specific experiences: Vibe Studio (App Maker), Forms Studio (Field Service Manager), Admin Portal (IT Admin).

**Target**: 550 existing Resco enterprise customers (550–2,200 IT Managers + Field Service Managers) as primary market; new customer acquisition as secondary driver.

**Revenue**: €100/user/month + AI credits consumption | 20 paying users by end of 2026 = ~€24K ARR seats; €2,400/year per average account (2 seats); scales to €220K ARR at 10% installed base penetration.

**Investment**: Infrastructure + GTM (core product built); TBD — requires cost baseline for cloud IDE containers and AI model costs.

**Strategic Value**: Transforms Resco from a mobile app platform into an AI-powered development ecosystem; creates switching costs; positions Studio as a new customer acquisition driver against Microsoft, Salesforce, and ServiceNow AI builders.

**Risks**: Value (Medium) — WTP at €100/month unvalidated | Usability (Medium) — trust barrier for AI modifying live projects | Feasibility (Low) — core built, compliance certs outstanding | Viability (Low) — unit economics clear.

**Urgency**: HIGH — Microsoft Power Apps Vibe, Salesforce MAGE, and ServiceNow Build Agent all shipped in 2025–2026. The window to own "AI-native Resco development" is open now; it will narrow as platform vendors expand into field service mobile.

**Next Action**: 10 structured discovery interviews with IT Managers at existing 550 customers — validate WTP at €100/month and map enterprise compliance approval process.

---

## 1. Problem

**What**: Resco enterprise customers have no unified, AI-native way to build and manage their Resco deployments. Capabilities are split across Resco App Configurator (Woodford), Questionnaire Designer, and generic AI tools — none of which share context or understand the customer's actual Resco project.

**Impact**:
- IT Managers spend hours on manual Woodford configuration, then switch to ChatGPT for JavaScript generation — getting generic output that doesn't understand their data model, entity structure, or workflows
- Field Service Managers depend on IT for every form change — creating bottlenecks between people who know what the field needs and people who can build it
- New capabilities (MCP setup, AI agent workflows, home replacements) have no self-service path — customers call or email Resco support
- Resco support carries operational burden for tasks that should be self-service

**Severity**: Must-have for AI-forward customers actively using or evaluating competitor platforms; Should-have for the installed base overall.

**Evidence**: IT Managers at Resco customers are already using ChatGPT alongside Woodford to generate JavaScript — a confirmed workaround that proves the problem is real. The workaround exists because no better tool does. The gap between "what AI could do with Resco context" and "what ChatGPT does without it" is the product's core value.

---

## 2. Target Customer

**Primary — App Maker (IT Manager)**:
IT Managers at Resco enterprise customers. Responsible for configuring and building Resco mobile apps, maintaining integrations with Dynamics 365, Salesforce, or ServiceNow, and managing field service application logic. Currently uses Woodford + external AI tools. Tech-savvy but not necessarily a professional developer.

**Secondary — Field Service Manager**:
Operations/Field Service Managers who own field worker processes. Need to create and iterate on inspection forms, work order questionnaires, and checklists for technicians — but currently depend on IT to execute every change. Non-technical; responds to "no IT ticket required" value prop.

**Tertiary — IT Admin (v2)**:
System administrators managing Resco licensing, user access across org units, and compliance/audit requirements. Needs self-service for what today requires Resco support calls.

**Market**:
- Installed base: 550 enterprise customers × 1–4 IT Managers = 550–2,200 direct users
- Seat expansion: 550 customers × 1–3 Field Service Managers = additional 550–1,650 seats
- Combined addressable seats (installed base): ~1,100–3,850 users
- New acquisition: TBD — Resco's broader addressable market in field service enterprise (research required)

**Accessibility**: Direct via Resco CSM and account management team across all 550 customers; Resco partner network; Resco developer community and documentation portal.

---

## 3. Opportunity Size

**Market**:
- TAM: Enterprise field service management software — $6.3B globally (2024, growing 12% CAGR) — TBD research required for precise Studio-relevant segment
- SAM: Resco's installed base — 550 enterprise customers, ~3,850 addressable seats
- SOM Year 1: 50 active users, 20 paying = €24K ARR seats + AI credits

**Revenue** (hybrid seat + consumption model):

| Scenario | Users | MRR (seats) | ARR (seats) | Notes |
|---|---|---|---|---|
| 2026 target | 20 paying | €2,000 | €24,000 | + AI credits |
| 5% installed base | ~110 users | €11,000 | €132,000 | + AI credits |
| 10% installed base | ~220 users | €22,000 | €264,000 | + AI credits |
| 20% installed base | ~440 users | €44,000 | €528,000 | + AI credits |

**Per-account economics**: 2 seats (1 IT Manager + 1 Field Service Manager) × €100/month × 12 months = **€2,400/year** per account, before AI credit consumption.

**AI credits upside**: Usage-based revenue on top of seats. Scale depends on consumption patterns — TBD until first 20 paying users establish baseline.

**Investment**: Core product built. Primary ongoing costs: cloud IDE container infrastructure, AI model API costs, security certification (SOC2), GTM (CSM enablement). Full cost baseline TBD.

**Strategic Importance Beyond Revenue**:
1. Acquisition driver — "the platform that builds itself" is a new Resco sales motion
2. Switching cost creator — Notes, template library, and project context make leaving Resco significantly more painful
3. Competitive defense — prevents Resco customers from migrating to Salesforce/MS platforms that now offer AI builders natively

---

## 4. Alternatives & Differentiation

**Current alternatives (how customers solve today)**:

1. **Resco App Configurator (Woodford) + ChatGPT/Copilot** — functional workaround but no project context, manual prompt engineering every session, generic JavaScript output requiring debugging, no integration between tools
2. **Resco Questionnaire Designer** — standalone forms tool, no AI, no connection to app configuration context, requires IT involvement for every change
3. **Resco support calls/email** — for new capabilities (MCP setup, home replacements, license changes) with no self-service path; slow, creates support backlog
4. **Do nothing / stay with Woodford** — accept the friction; lose no money but gain no new capability

**Competitor platforms** (relevant if customers consider platform migration):

| Competitor | AI Builder | Multi-Backend | Offline | Field Service Mobile | Resco-Native AI |
|---|---|---|---|---|---|
| **Microsoft Power Apps Vibe** | ✅ $20/user/month | ❌ MS only | ⚠️ Coming 2026 | ⚠️ Limited | ❌ |
| **Salesforce MAGE** | ⚠️ Scaffold only, needs devs | ❌ SF only | ⚠️ Manual SDK | ⚠️ Limited | ❌ |
| **ServiceNow Build Agent** | ✅ Full app gen | ❌ SN only | ❌ No native offline | ⚠️ Limited | ❌ |
| **Resco Studio** | ✅ Full project modification | ✅ Dataverse/Dynamics/SF/SN | ✅ 18 years production | ✅ Core use case | ✅ Only option |

**Key differentiation**:
- **vs Woodford+ChatGPT**: Resco-native AI eliminates manual context injection; modifies the actual project; no context switching; reusable template library
- **vs Microsoft/Salesforce/ServiceNow AI builders**: Multi-backend support (they are each single-ecosystem); proven offline; no compilation step; Resco project context none of them have or can replicate
- **vs all competitors**: No one else builds tools for Resco projects because no one else is Resco

---

## 5. Why Us

**Strategic fit**:
Resco Studio is a natural extension of Resco's core business — it deepens the platform moat while creating a new recurring revenue stream. Resco owns every asset needed to build it: the project schema, the JSBridge documentation, the mobile container, the customer relationships, the field service domain expertise. No third party can replicate Resco-native AI without years of Resco-specific training data.

**Unique capabilities**:
1. **Own the project schema** — Resco has direct API access to customer project structure; no external AI can match this context without significant integration complexity
2. **18 years of Resco customer patterns** — the UI template library is built on real deployments; no competitor starts with this asset base
3. **Multi-backend runtime** — Dynamics 365, Salesforce, ServiceNow, Dataverse in a single Resco deployment; competitor AI builders are each single-ecosystem
4. **No-compilation mobile deployment** — describe → generate → runs on device; no Xcode, no Android Studio, no app store submission; competitors cannot match this without abandoning their native app architecture
5. **Existing CSM relationships** — direct access to 550 enterprise customers for beta, feedback, and rollout; no cold GTM required
6. **MCP foundation already built** — Resco MCP server is live and proven; Studio extends it into a managed UI

**Unfair advantage**: Resco owns the runtime. Competitors build AI tools that generate code; Resco builds an AI tool that directly modifies a live deployment. The gap between "generates code you then deploy" and "modifies your project directly" is large — and only Resco can offer the latter for Resco projects.

---

## 6. Why Now

**Market timing**:
Microsoft, Salesforce, and ServiceNow all shipped AI app builders in 2025–2026. Enterprise customers are now actively evaluating AI-native development tools. Resco customers will ask: "why doesn't Resco have something like this?" The question is already forming. Shipping now positions Resco as a leader; shipping in 12 months positions Resco as a follower.

**Technology enablers**:
MCP (Model Context Protocol) emerged as a standard in 2025, enabling AI agents to connect to external tools in a structured way. Resco MCP server is already live. Container-based cloud IDEs (VS Code Server, Cursor) have matured to the point where a Resco-specific Cloud IDE is feasible without building a browser-based code editor from scratch. LLM context windows are large enough (200K+ tokens) to hold an entire Resco project in context.

**Competitive threat**:
The 2025–2026 window is when enterprise customers are forming new habits around AI development tools. Customers who adopt Microsoft/Salesforce AI builders now will build muscle memory and workflows around those tools — making them harder to retain long-term. Resco must be in the consideration set before habits solidify.

**Customer readiness**:
Confirmed: IT Managers at Resco customers are already using ChatGPT alongside Woodford. They are not waiting for AI — they are already using it, poorly. The demand exists today; the question is whether they get a good Resco-native experience or continue with a bad generic workaround.

**Urgency**: HIGH — first-mover window in "AI for Resco development" is 3–6 months before platform vendors deepen their field service mobile coverage.

---

## 7. Go-to-Market

**Strategy**: Land in existing base (low CAC, high trust), then use Studio as acquisition driver for new logos.

**Phase 1 — Closed Beta (May–July 2026)**:
10 existing customers identified by CSM team as early adopters (IT Managers already using AI tools for Resco customization). Structured feedback program. Goal: validate AI output quality, identify compliance blockers, refine onboarding.

**Phase 2 — GA to Installed Base (August–September 2026)**:
General availability to all 550 existing Resco customers. CSM-led introduction: demo, trial offer, pricing conversation. Goal: 50 active users, 20 paying by December 2026.

**Phase 3 — Acquisition Motion (Q4 2026 onwards)**:
Studio becomes a named feature in Resco new business sales. "The only field service mobile platform with an AI that knows your project" is the acquisition headline. Resco partner network trained on Studio value proposition.

**Channels**:
- Primary: Resco CSM team — direct outreach to 550 existing accounts
- Secondary: Resco partner network — partners who build Resco deployments for customers are power users of Studio (App Maker persona)
- Organic: Resco developer documentation, community portal, YouTube tutorials on Vibe Studio builds
- Eventual: Marketplace listings (Microsoft AppSource, Salesforce AppExchange) for acquisition

**Viral loop**: Home replacements and form templates built in Studio become shareable — a customer who shares a template drives another customer to open Studio to use it. Library grows as a community asset.

---

## 8. Success Metrics

**Primary (North Star)**: Monthly Active Users completing at least one AI-driven project modification or form creation in Studio.

**2026 Decision Gates**:

| Timeframe | Metric | Target | Action if missed |
|---|---|---|---|
| End of closed beta (July 2026) | Beta users completing first modification | 7/10 | Fix onboarding before GA |
| GA launch (September 2026) | Active users | 25 | Investigate adoption blockers |
| End of 2026 | Paying users | 20 | Re-evaluate pricing / trial conversion |
| End of 2026 | ARR (seats) | €24,000 | Adjust GTM approach |

**Supporting metrics**:
- Activation rate: % of trialing users who complete first AI modification within 30 minutes
- 30-day retention: % of activated users still active after 30 days
- Seats per account: target >1 (indicates Field Service Manager persona adoption alongside IT Manager)
- AI credits consumed per active user/month (establishes consumption revenue baseline)
- Net new Resco customers citing Studio in deal notes (acquisition attribution)
- Support ticket deflection: reduction in Resco support tickets for tasks now self-service in Studio

---

## 9. Critical Success Factors

**Dependencies**:
1. **Security certification** — SOC2 Type II (or equivalent) must be in progress or completed before enterprise procurement approval. Without it, IT security teams at large enterprise accounts will not approve Studio regardless of product quality. This is the single biggest external dependency.
2. **CSM enablement** — Resco CSM team must be trained, equipped with demo scripts, and incentivized to introduce Studio to existing accounts. Studio will not sell itself to 550 customers without active CSM involvement.
3. **AI output quality bar** — the first 10 beta users must get correct, project-appropriate AI output on first use. One high-profile failure (AI breaks a production Resco deployment) will spread through the Resco customer community and undermine trust that takes months to rebuild.
4. **Onboarding to first value in <30 minutes** — if IT Managers cannot experience a meaningful AI modification within 30 minutes of first login, trial-to-paid conversion will be low regardless of product capability.

**Required capabilities**:
- Preview/diff before applying AI changes — essential for trust; users must see what the AI will do before it does it
- Rollback capability — undo any AI-generated modification; reduces perceived risk of trying the product
- Sandboxed trial environment — allows IT Managers to experience Studio without connecting their live production Resco project (removes security hesitation during evaluation)
- SSO/SAML support — enterprise IT teams require SSO as baseline for approval; without it, Studio cannot be deployed organization-wide

---

## 10. Risks (SVPG Four Risks)

### Value Risk: Will customers buy and use this?
**Level**: Medium

**Why Medium, not High**:
The problem is confirmed real — IT Managers are already using workarounds. The solution is working and differentiated. The risk is not whether the product is valuable but whether customers will pay €100/month for value they currently get imperfectly for free (ChatGPT is included in many enterprise agreements). Confirmed evidence of workaround behavior reduces value risk from High to Medium.

**Specific value risks**:
- €100/month price point is unvalidated; ChatGPT+Woodford exists as free alternative
- "Resco-native AI is better" claim requires demonstration — customers must experience the difference to believe it
- Field Service Manager persona (Forms Studio) has clearer ROI story ("no IT ticket") than IT Manager persona — risk is lower for FS Manager adoption

**Mitigation**:
- 10 customer discovery interviews THIS MONTH — direct WTP validation at €100/month
- Build ROI calculator: time saved on Resco customization × hourly rate = payback period at €100/month
- Free trial with AI credits included — let customers experience the quality difference before paying
- Lead with Forms Studio in demos for mixed IT/FS Manager audiences — cleaner value story, faster conviction

---

### Usability Risk: Can users figure it out?
**Level**: Medium

**Why Medium**:
Natural language interfaces reduce learning curve vs traditional configuration tools, but two specific usability challenges exist. First, IT Managers must trust an AI to modify their live production Resco project — a high-stakes action that creates psychological friction regardless of how good the AI is. Second, three distinct persona experiences (Vibe Studio, Forms Studio, Admin Portal) must each feel immediately intuitive for a non-developer audience.

**Specific usability risks**:
- "AI will break my live project" fear blocks first use — even technically capable users hesitate before irreversible-seeming actions
- Field Service Manager persona is non-technical; Forms Studio must work without any Resco configuration knowledge
- Notes (Notebook LLM) is an unfamiliar interaction model — users may not understand how to use it productively without guidance

**Mitigation**:
- Preview/diff UI is mandatory before any AI modification applies — show exactly what will change before it changes
- Rollback on every modification — make "undo" visible and prominent
- Sandboxed environment for first-time users — allow full Studio experience with a sample project before connecting live deployment
- Forms Studio must be zero-Resco-knowledge — if a Field Service Manager needs to understand Resco to use Forms Studio, the design has failed

---

### Feasibility Risk: Can we build it?
**Level**: Low

**Why Low**:
The core product is built and working. AI Project Modifier, MCP Hub, and Forms Builder are all functional today. The remaining feasibility work is infrastructure hardening and compliance certification — neither of which requires novel technical invention.

**Remaining technical work**:
- SOC2 Type II certification process (operational, not technical — but requires time and process investment)
- Multi-tenant container infrastructure for cloud IDE at scale (known engineering challenge, not unknown)
- SSO/SAML integration (standard enterprise identity requirement)
- Preview/diff and rollback UI (product design challenge, not technical breakthrough)

**Open technical questions** (from Feature Business Value Map):
1. **Notes depth**: Is Notes read-only (AI explains the project) or read-write (AI modifies from Notes context)? Read-write is significantly more complex and carries higher quality risk.
2. **Forms vs App Builder overlap**: Can App Builder already build questionnaires, making Forms Studio purely a UX scoping exercise? If yes, Forms Studio complexity is Low. If a separate AI model tuning is needed, complexity rises.
3. **MCP Hub scope at launch**: Which 3rd party MCPs are supported? Curated list of 10 vs "any MCP" changes QA burden significantly.
4. **AI credits unit pricing**: Per token, per operation, or per session? This affects infrastructure cost modeling and billing system requirements.

---

### Business Viability Risk: Does it work for Resco's business?
**Level**: Low

**Why Low**:
Unit economics are clear and favorable at scale. The product is built — sunk cost is already spent. Incremental revenue from even 5% installed base penetration (€132K ARR) covers ongoing infrastructure and GTM costs. The strategic value (acquisition driver, switching cost, competitive defense) justifies investment independent of direct Studio revenue.

**Viability considerations**:
- €100/month pricing needs validation but the range (€50–€150) is supported by comparable enterprise productivity tools
- AI credit consumption revenue is upside with uncertain floor — requires 20+ paying users to establish consumption baseline
- Resco's CSM team is the primary GTM lever; Studio success depends on CSM bandwidth and incentive alignment
- The 2026 target (20 paying users / €24K ARR) is conservative by design — achievable with modest CSM effort from 550-customer base

**Break-even estimate**: TBD until infrastructure cost baseline established. At €100/user/month, break-even is the number of users whose seat revenue covers monthly infrastructure + AI model costs + allocated CSM time. Hypothesis: break-even at 30–50 paying users.

---

## Recommendation

**Decision**: ✅ **PURSUE** — proceed to closed beta immediately

**Rationale**:
- ✅ Core product is built — investment already made; opportunity cost of not launching is high
- ✅ Differentiation is real and durable — Resco-native AI context cannot be replicated by any competitor; multi-backend + no-compilation advantage is confirmed vs Microsoft, Salesforce, ServiceNow
- ✅ Problem is confirmed — IT Managers are using ChatGPT+Woodford workaround today; demand exists, not just hypothesized
- ✅ Market timing is right — competitor AI builders just shipped; window to own "AI for Resco" is open now and will narrow
- ⚠️ Price point needs validation — €100/month is a hypothesis; discovery interviews must confirm WTP before full GA pricing is locked
- ⚠️ Compliance barrier must be mapped — enterprise security approval timeline is unknown; must be characterized before enterprise rollout plan is credible
- ✅ Strategic value justifies investment even at conservative ARR — acquisition driver + switching cost + competitive defense exceed direct Studio revenue in strategic importance

**One-sentence recommendation**: Resco Studio is a built, differentiated, strategically critical product with confirmed demand — the only remaining questions are price validation and compliance path, both solvable through a structured 10-customer discovery sprint before GA.

---

## Biggest Risk & Test Plan

**Risk**: Enterprise IT security/compliance teams block Studio as a 3rd party cloud tool accessing production Dynamics/Salesforce/ServiceNow environments — preventing adoption before pricing even becomes relevant. (High)

**Combined threat**: If compliance blocks adoption AND €100/month faces WTP resistance simultaneously, Studio is left with only technically sophisticated, budget-flexible early adopters — a small segment that delays reaching the 20-paying-user target.

### Validation Plan

**THIS MONTH (May–June 2026)**: 10 structured discovery interviews with IT Managers at existing Resco customers.

**Setup**:
- CSM team identifies 10 IT Managers known to use external AI tools for Resco customization (highest likelihood of early adoption)
- 30-minute structured interview: 15 min live Vibe Studio demo → 10 min WTP conversation → 5 min compliance mapping
- Interview guide covers: current workflow, time spent on Resco customization, reaction to demo, pricing reaction at €100/month, compliance approval process and timeline

**Measure**:
- WTP: % who say "yes" or "probably yes" to €100/month → target 6/10
- Compliance path: characterize approval process at each account (days, approvers, requirements)
- Activation intent: % who want to join closed beta → target 5/10

**Decision (end of June 2026)**:
- ✅ 6+/10 WTP confirmed + compliance path <90 days at most accounts → proceed to closed beta July, GA September
- ⚠️ 4–5/10 WTP OR compliance >90 days majority → adjust pricing to €50/month trial tier OR prioritize SOC2 + SSO before GA
- ❌ <4/10 WTP OR compliance universally blocking → pause GA, run deeper pricing research, re-scope v1 to lowest-compliance-friction capabilities first

**Why critical**: Every day without this data, GTM and pricing decisions rest on assumptions. These 10 interviews convert the two biggest risks from "unknown" to "managed" or "mitigated" — unlocking confident investment in GA launch.

**Backup plan**: If enterprise compliance universally blocks Studio, launch a sandboxed "Studio Lite" tier with no connection to live production environments — AI works against synthetic/sample Resco projects, proving value without triggering security review. Use Studio Lite to build product trust and build compliance dossier in parallel.

---

## Next Steps & Timeline

### May–June 2026: Discovery Sprint
CSM team runs 10 structured discovery interviews. Deliverable: WTP validation + compliance barrier map. Decision gate: pursue GA timeline or adjust.

### July 2026: Closed Beta
5–10 willing customers from discovery sprint. Structured feedback: onboarding time-to-value, AI output quality, trust/hesitation moments, feature gaps. Deliverable: closed beta report with specific onboarding and quality improvements.

### August 2026: GA Readiness
SOC2 in progress documentation ready for security reviews. SSO/SAML live. Preview/diff and rollback UI complete. CSM demo playbook and ROI calculator ready. Pricing confirmed from discovery data.

### September 2026: GA Launch
General availability to all 550 existing Resco customers via CSM-led outreach. 30-day free trial with AI credits. Target: 25 active users by end of October.

### Q4 2026: First Revenue Gate
Target 20 paying users by December 2026. If on track: begin acquisition motion — Studio enters Resco new business sales playbook. If behind: diagnose conversion gap (trial quality, pricing, compliance) and address before acquisition push.

**Critical path**: Discovery interviews → compliance path known → closed beta → onboarding fixes → GA → 20 paying users → acquisition motion.

---

## Key Assumptions & Open Questions

**Assumptions requiring validation**:
1. IT Managers will pay €100/month for Resco-native AI vs free ChatGPT+Woodford alternative
2. Enterprise security teams have an approvable compliance path for Studio within 90 days
3. AI output quality is high enough to earn trust on first use without breaking production projects
4. Forms Studio is sufficiently scoped for non-technical Field Service Managers without Resco knowledge
5. CSM team has bandwidth and incentive to introduce Studio to 550 customers in 2026
6. 30-minute onboarding to first value is achievable with current UX
7. Notes (Notebook LLM) is in v1 read-only scope — not read-write modification

**Open product questions** (from Feature Business Value Map):
1. Notes depth: read-only explanation vs read-write modification — decide before closed beta
2. Forms vs App Builder scope boundary — define to prevent persona confusion in demos
3. MCP Hub launch scope: curated 3rd party MCP list vs open "any MCP" — define for QA planning
4. AI credits unit pricing: per token / per operation / per session — needed for infrastructure cost modeling

**Contingency**:
If compliance is universally blocking: launch Studio Lite (sandboxed, no live project connection) as free product → build compliance dossier while proving value → upgrade path to full Studio once security approved.

**Potential outcomes**:
- **Best**: 10% installed base by end of 2026 = 220 users = €264K ARR + credits; becomes acquisition driver in 2027
- **Good**: 20 paying users by end of 2026 = €24K ARR; compliance path clear; GA momentum building
- **Acceptable**: 10 paying users; compliance blocking 50% of accounts; adjust pricing or launch Studio Lite
- **Failure**: <5 paying users; WTP not validated at any price point; compliance universally blocking

---

**Reviewed by**: — | **Approval**: Pending | **Next review**: After 10 discovery interviews (end of June 2026)
