# Lean Canvas: RESCO AI Vibe Studio

**Date**: 2026-02-08 | **Company**: RESCO | **Version**: 3.0 | **Status**: Validated + Independently Challenged

---

## 📋 Executive Summary

**Idea**: AI-powered web studio (vibe.resco.net) that lets new prospects and business app makers build complete enterprise mobile apps through natural language — running inside Resco's proven offline-first mobile container with multi-backend support. "Build business apps when others fail."

**Target**: New prospects from MS Dynamics (~5,000 partners), Salesforce (~3,400 partners), and ServiceNow (~1,300 partners) ecosystems who need offline-first mobile apps but face high barriers to entry with current tools

**Economics**: €185-285K Year 1 (2.5 FTE + LLM + infra), hybrid revenue: $70-100/month Vibe Studio subscription + $10/user/month Resco license (primary). Stress-tested Year 1 revenue: €44-103K (realistic) to €153-363K (optimistic). Break-even likely Year 2 under realistic assumptions.

**Risk**: AI-generated code quality must earn trust on first try with users who can't fix it manually; Microsoft's vibe.powerapps.com is already live and expanding globally; Salesforce MAGE launched Feb 2026 targeting the same segment

**Next Action**: Build MVP (Month 1), closed beta with new prospects on real use cases (Month 2-3), measure time-to-first-app and Resco license conversion

---

## 🎯 Problem

### Top 3 Problems (Priority Order)
1. **High skill barrier blocks new customer acquisition**: Resco Woodford is proprietary and unique — every new prospect must invest significant time mastering it before they can build anything. This blocks growth. New partners/customers who are experienced in Microsoft, Salesforce, or ServiceNow stacks cannot easily adopt Resco. (Source: partner feedback, customer interviews, internal observations)
2. **Slow build-test-deploy cycle**: Even for those who can build, creating Resco mobile apps requires manual Woodford configuration + coding + sync + device testing — a cycle that takes hours-to-days per iteration with no live preview capability. (Source: partner feedback, experience)
3. **Competitors offer modern AI-assisted tooling**: vibe.powerapps.com and other platforms now offer AI-generated apps. Resco has no equivalent — risking perception as outdated among new prospects evaluating platforms

### Existing Alternatives
- **Woodford** (Resco's config tool): Powerful but steep learning curve, no live preview, requires deep expertise — works for existing partners, blocks new ones
- **Power Apps** ($20/user/month premium, $10/user/app/month pay-as-you-go since Jan 2026): AI-assisted via vibe.powerapps.com (live, expanding globally), but Microsoft-only backend, limited offline (cloud flows don't work offline, no default data encryption, sync filter complexity), no native mobile experience out of the box
- **Salesforce MAGE** (launched Feb 2026): Mobile App Generation Ecosystem — generates production-ready native mobile code from natural language. Salesforce-only backend, but directly targets the SF ecosystem segment Resco wants to capture
- **Salesforce Mobile SDK / ServiceNow Mobile Studio**: Platform-locked, offline-first remains a "pro-code effort" (Forrester)
- **Lovable / Bolt / v0**: AI vibe coding platforms with massive traction (Lovable: $200M ARR, $6.6B valuation). Generate generic web apps — no enterprise offline, no CRM integration, no field-service specialization
- **Generic AI coding tools** (ChatGPT/Copilot): Hallucinate Resco APIs, no backend schema access, no device preview

---

## 👥 Customer Segments

**Primary**: New prospects — implementation partners and consultants experienced in Microsoft D365, Salesforce, or ServiceNow who need offline-first mobile app capabilities but don't know Resco Woodford. Vibe Studio is their **entry point** into the Resco ecosystem, skipping Woodford entirely.

**Secondary**: Existing Resco partners building quick, simple solutions (e.g., external user apps, simple data capture) — use cases that don't require robust workflows or deep Woodford expertise. For complex projects, existing partners use Woodford + MCP server.

**Market size**:
- **TAM**: ~10,000+ implementation firms (MS D365 ~5,000 + Salesforce ~3,400 + ServiceNow ~1,300) + tens of thousands of individual consultants | Low-code platform market ~$45-52B in 2026, 19% CAGR (Source: Fortune Business Insights, Gartner) | Field service market $5-9B growing 11-16% CAGR (Source: MarketsandMarkets, Mordor Intelligence, GM Insights)
- **SAM**: Firms needing offline-first mobile — Gartner projects 60%+ of field service orgs will implement in-field mobile apps within 3 years, yet most platforms offer limited or no offline. On-premises/offline deployment models represent ~38% of market share, driven by uninterrupted data access needs (Source: Gartner, industry reports). ⚠️ *Note: The specific "60% need / 30% supply" gap claim could not be independently verified in public sources. The directional insight (high offline demand, low offline supply) is supported by multiple industry analysts, but the exact figures should be cited with caution or sourced internally.*
- **SOM (Year 1)**: See Conversion Funnel Analysis below — realistic range: 42-84 new entries (2-3x current baseline)

### 📊 Conversion Funnel Analysis (replaces 5x growth assumption)

Here is a funnel-based estimate:

| Funnel Step | Metric | Conservative | Moderate |
|-------------|--------|-------------|----------|
| Website visitors (vibe.resco.net) | Annual unique visitors | 3,000 | 6,000 |
| → Register (get 5 free credits) | ~7% conversion | 210 | 420 |
| → Build a working app | ~30% of registrations | 63 | 126 |
| → Try app on device (QR preview) | ~50% of app builders | 32 | 63 |
| → Deploy to production | ~20% of device testers | 6 | 13 |
| → Purchase Resco licenses | ~80% of deployers | 5 | 10 |

**Implications**: To reach even 10 production deployments in Year 1, you need ~6,000 relevant website visitors. This requires active marketing — organic discovery of a niche B2B tool will not generate this volume alone.

⚠️ **The original 140 entries (5x) assumption requires ~12,000+ annual visitors with above-average conversion at every step. Treat as aspiration, not forecast.**

**Reachability**: Resco partner account managers (16 active partners) | vibe.resco.net organic signups (new channel) | Microsoft Dynamics / Salesforce / ServiceNow LinkedIn groups and forums | Resco events and conferences

**Current acquisition baseline**: ~8 new partners/year + ~20 new customers/year = 28 new entry points (without Vibe Studio)

---

## 💎 Unique Value Proposition

**"The only AI app builder that builds offline apps that works offline, with any CRM backend."**

**Full statement**: "We help business app makers build enterprise mobile apps with AI — running inside Resco's proven offline-first container with multi-backend support and enterprise-grade security. No mobile infrastructure to build. No platform lock-in. No Woodford expertise needed."

**High-level concept**: "Like vibe.powerapps.com, but your app works offline and connects to any CRM backend — not just Microsoft"


**Why different**:
- vs **Power Apps / vibe.powerapps.com**: Offline-first with encrypted local data (proven by 2,500+ customers), multi-backend (not Microsoft-only). Power Apps: cloud flows don't execute offline, no default data encryption, limited sync control. Pricing: Resco $10/user/month vs Power Apps $10-20/user/month (pay-as-you-go vs premium) — price parity on low end, advantage on high end
- vs **Salesforce MAGE** (NEW — launched Feb 2026): Salesforce-only backend. Resco is platform-agnostic. MAGE generates SF-native mobile code; Resco generates cross-platform offline-first apps. Key differentiator: Resco works with SF AND D365 AND ServiceNow
- vs **Salesforce Mobile SDK / ServiceNow Mobile Studio**: Platform-locked, offline-first remains a "pro-code effort" (Forrester)
- vs **Lovable / Bolt / v0**: Output runs in enterprise-grade Resco mobile container with security, sync, and offline — not a generic web app. These platforms generate impressive demos but lack enterprise offline, CRM integration, and field-service specialization
- vs **Woodford**: AI-generated, no learning curve, live preview — accessible to newcomers who've never seen Woodford

**Why now**: "Vibe coding" is mainstream (Collins Word of the Year 2025, 87% of Fortune 500 use vibe coding platforms, 92% of US devs use AI tools daily). High offline demand with low platform supply in field service. Microsoft pushing AI-assisted development (vibe.powerapps.com already live) = market window for Resco to capture multi-backend offline-first position before competitors close the gap. **Window is 6-12 months.**

---

## ✨ Solution

### Top 3 MVP Features (Phase 1 — UIReplacement, New Customer Acquisition)
1. **Frictionless onramp**: Register at vibe.resco.net → get 5 free credits → start immediately with RescoCloud sandbox (pre-configured demo backend, zero setup) OR connect own backend (Dataverse, Salesforce, ServiceNow) → create mobile project
2. **AI-powered full app generation**: Describe app in natural language → AI (Claude/LLM via Resco MCP server, pre-configured by Resco) generates complete UIReplacement code → displayed in Monaco editor with real-time progress → iterate with prompts or manual edits. User focuses on business logic — Resco container provides offline sync, security, and mobile experience automatically
3. **QR-based live device preview + publish**: Scan QR → app appears on physical device → auto-refreshes on code changes (live dev mode) → publish to production when ready, continue developing

### Delivery Channel
Web application at vibe.resco.net (browser-based, no local installation). AI/LLM provided by Resco's pre-configured environment (user does not bring own API key — credits cover AI costs).

### Guided Deployment Path (CRITICAL for revenue conversion)

⚠️ **The demo-to-production gap is the #1 revenue risk.** Every vibe coding tool (Lovable, Bolt, v0) struggles with users building demos but never shipping to production. For Resco, the gap is worse because production requires Resco licenses, backend config, sync setup, and security policies — none of which the AI handles.

**Recommended MVP addition**: After a user builds and previews an app, provide a guided deployment wizard:
1. **"Ready to deploy?"** prompt after successful QR preview
2. **Automated production checklist**: backend connection verified → sync filters configured → security policies applied → license requirement explained
3. **Partner handoff option**: connect the user with a Resco partner for assisted deployment (partner gets a warm lead, user gets expert help)
4. **Self-service path**: step-by-step guided wizard for simple deployments

### Template Library (alongside freeform generation)

⚠️ **AI freeform generation has a first-try failure risk.** Templates with AI customization will have much higher success rates than pure NL-to-code for new users who can't debug failures.

**Recommended**: Ship 5-10 industry-specific templates at launch:
- Field service inspection form
- Work order management
- Asset check / inventory
- Field sales visit report
- Property inspection
- Delivery route / proof of delivery

Each template: fully working baseline → user customizes via AI prompts ("add a photo capture field", "change the layout to tabs") → much higher first-try success rate.

### NOT in MVP
- Form Components (visible but disabled — Phase 2)
- AI Assistants / AI Pantheon (visible but disabled — Phase 2+)
- Questionnaire builder (visible but disabled — Phase 2+)
- List Components (TBD)
- Marketplace for tools/snippets (future)
- Multi-user collaboration (future)
- RescoCloud as production backend (demo/trial only in Phase 1)
- Additional backends: Zoho, HubSpot, others (Year 2-3)

---

## 🔑 Unfair Advantage

### 💪 Core Strengths (validated)

**The intersection of three capabilities no competitor matches:**

| Capability | Resco | Power Apps | SF MAGE | Lovable | Mendix |
|------------|-------|------------|---------|---------|--------|
| Offline-first (native) | ✅ | ❌ Limited | ❌ SDK-level | ❌ | ⚠️ Partial |
| Multi-backend (D365+SF+SN) | ✅ | ❌ MS only | ❌ SF only | ❌ | ✅ |
| Field service specialized | ✅ | ⚠️ One of many | ⚠️ One of many | ❌ Generic | ⚠️ Horizontal |
| AI app generation | 🔜 Planned | ✅ Live | ⚠️ Preview | ✅ $200M ARR | ✅ In prod |

**No single competitor matches all three core capabilities (offline + multi-backend + field-service).** This is Resco's genuine moat. BUT — Resco is also the only one that hasn't shipped AI app generation yet. Speed to market is critical.

### Moat Analysis

**Platform owner moat**: Only Resco can build deeply integrated AI code generation for its own mobile container — proprietary access to Woodford metadata APIs, mobile project structure, offlinehtml deployment pipeline, sync infrastructure. Third parties cannot replicate this.

**Proven mobile container**: ~2,500 corporate customers running Resco offline-first mobile apps in production with ~200K+ licensed users. The generated code inherits enterprise-grade security (encrypted local data by default), offline sync (up to 10x faster than alternatives), and native mobile experience without the developer building any of it.

**Multi-backend (the Microsoft-proof moat)**: Resco works with Dataverse, Salesforce, ServiceNow, and more coming. Microsoft will never support non-Microsoft backends. Salesforce will never support non-Salesforce backends. This is the differentiator that survives even if Microsoft closes the offline gap AND Salesforce improves MAGE.

**MCP server synergy**: Already in development — provides the AI context layer (JSBridge docs, backend schemas, sync analysis) that makes code generation accurate. Shared investment with separate initiative. MCP ecosystem is mature (97M+ monthly SDK downloads, 5,800+ servers, native Copilot Studio support).

**Captive distribution**: 16 active partners + direct account manager relationships = built-in beta channel and go-to-market.

---

## 📊 Channels

**Primary**: vibe.resco.net organic signups (new channel — frictionless try with 5 free credits) + Resco partner account managers for direct outreach

**Early adopters**: New prospects from MS D365/Salesforce/ServiceNow ecosystems evaluating mobile solutions + existing partners wanting quick simple solutions

**Community/Content**: "Build an app in 5 minutes" demo videos | Microsoft Dynamics / Salesforce / ServiceNow LinkedIn groups | Resco annual conference | Partner technical forums | Resco documentation site

**Launch strategy**: Month 1-2 build MVP → Month 2-3 closed beta (10-15 users, mix of new prospects and existing partners) → Month 4-5 open beta → Month 6 public launch at vibe.resco.net

**Viral loop**: Prospect tries free credits → builds working app → demos to their client → client wants production deployment → Resco license sale → consultant recommends Vibe Studio to peers

---

## 💰 Economics

**Revenue model**: Hybrid (dual-stream)
- **Direct**: Vibe Studio subscription ~$70-100/month (hybrid: included credits + usage overage for AI turns). 1 credit = 1 AI conversation turn.
- **Indirect (primary)**: Resco Mobile CRM licenses at $10/user/month when Vibe Studio-built apps go to production. This is the North Star revenue.
- **Onramp**: 5 free credits at registration (no payment required to try)

**Pricing context**: Resco $10/user/month vs Power Apps $10-20/user/month (pay-as-you-go $10/user/app since Jan 2026, premium $20/user). 

**Per-project revenue** (indirect): 20 users (avg) × $10/month × 24 months retention = $4,800 per project

**Investment** (2.5 FTE team):
- Build: 2.5 FTE × 6 months = €75-100K
- LLM API costs: €30-60K/year (scales with usage)
- Infrastructure: €30-50K/year (RescoCloud sandbox, hosting, preview)
- Maintenance (post-launch): €50-75K/year (same 2.5 FTE)
- **Total Year 1**: €185-285K

**Revenue forecast (Year 1)** — original vs stress-tested:

| Stream | Original Conservative | Original Moderate | ⚠️ Stress-Tested Realistic |
|--------|----------------------|-------------------|---------------------------|
| New entries/year | 140 (5x) | 140 (5x) | 42-84 (2-3x, funnel-based) |
| Deploy to production | 10% | 20% | 5-10% |
| Users per deployment | 20 avg | 20 avg | 10-15 (new prospects start small) |
| Direct (Vibe Studio subs) | ~€27K | ~€27K | ~€15-27K |
| Indirect (Resco licenses) | ~€126K | ~€336K | ~€17-76K |
| **Total** | **~€153K** | **~€363K** | **~€44-103K** |

**Break-even**: Original moderate scenario claimed Year 1 profitability. **Under stress-tested assumptions, break-even shifts to Year 2-3.** The investment (€185-285K) is still manageable, but budget for a 2-year payback period, not 1 year.

---

## 📈 Key Metrics

**North Star**: Resco license revenue directly attributable to Vibe Studio users — the ultimate proof this tool drives business

**Success criteria**:
- 6 months: 50 registrations, 15 active users, time-to-first-app < 1 hour
- 12 months: 200 registrations, 40 paid subscribers, 10 production deployments
- 12 months (North Star): 10 deployments × 20 users × $10/month = **$24,000 ARR in attributable Resco license revenue**

**Supporting metrics**:
- Time-to-first-app: < 1 hour (primary activation metric — if > 2 hours, product/UX problem)
- AI code generation success rate: > 70% runs without manual fixes
- Free → paid subscription conversion: target > 10%
- Live preview sessions per user per week: > 5 (engagement depth)
- WAU/MAU: > 40% (habit formation)

**Failure criteria**:
- 6 months: < 20 registrations or time-to-first-app > 2 hours → product/UX problem
- 12 months: < 5 production deployments → tool makes demos but not real apps
- 12 months: $0 attributable Resco license revenue → Vibe Studio doesn't convert to business

**Tracking**: Vibe Studio analytics (usage logs, credit consumption) | Resco CRM pipeline attribution (which licenses came via vibe.resco.net) | Partner surveys (quarterly NPS) | User interviews

---

## 🚨 Critical Risks

**Riskiest assumption**: AI-generated Resco code will be good enough on first try that a new prospect — who doesn't know Resco and can't fix code manually — trusts it and keeps going. You get one shot at first impression.

**Top 6 Risks**:

1. **🔴 AI code quality / First-Try Problem (HIGHEST)**: Generated UIReplacement code doesn't work reliably → new prospects (who can't debug Resco code) lose trust on first attempt and never return.
   - **Why this is underestimated**: Lovable ($6.6B valuation, $200M ARR) invested hundreds of millions to achieve reliable first-try generation. Resco is budgeting 2.5 FTE. The target users are non-Resco-experts by definition — when code fails, they literally cannot debug it. Every failure is a **permanent churn event**. The 70% AI success rate target means 3 out of 10 attempts fail — for a first-impression product, this may be too low.
   - *Mitigation*: MCP server provides context (confirmed mature). BUT context alone isn't enough — invest in: (a) **template library** with AI customization (higher success rate than freeform), (b) **curated starter patterns** for common use cases, (c) dedicated prompt engineering effort post-launch (minimum 1 FTE). Monaco editor as manual fallback, but remember: target users can't use it.

2. **🔴 Competition is closer than assumed (VERY HIGH)**: This is not a future threat — it's current reality.
   - **vibe.powerapps.com**: Already live in production preview, expanding globally. Microsoft's $10/user/app pay-as-you-go pricing eliminates Resco's previous price advantage.
   - **Salesforce MAGE** (NEW — Feb 2026): Mobile App Generation Ecosystem generates production-ready native mobile code from natural language. Directly targets the Salesforce ecosystem segment Resco listed as a primary target (~3,400 partners).
   - *Mitigation*: Speed to market. Lead with **multi-backend** (the one thing neither Microsoft nor Salesforce will ever do). Expand Vibe Studio capabilities (AI agents, components, questionnaires) to widen feature moat. **Competitive window: 6-12 months.**

3. **🟠 New prospect conversion / Funnel reality (HIGH)**: The original 5x growth assumption (28 → 140 entries/year) has no supporting data and is likely too optimistic.
   - **Funnel math**: With ~7% site-to-registration conversion, ~30% build-an-app rate, ~50% device-test rate, ~20% production-deploy rate, and ~80% license purchase rate — you need **~6,000 annual website visitors to get 10 production deployments**. Organic discovery of a niche B2B tool will not generate this volume alone.
   - *Mitigation*: Allocate marketing budget ($20-50K for LinkedIn campaigns, content marketing, partner co-marketing). Track registration source from day 1. Invest in "build an app in 5 minutes" demo content. Model and track the full funnel: visit → register → build → preview → deploy → license.

4. **🟠 Demo-to-production gap (HIGH — upgraded from MEDIUM)**: Users build cool demos with free credits but never deploy to production → $0 North Star revenue.
   - **Why this is the actual #1 revenue risk**: Every vibe coding tool struggles here. For Resco, the gap is worse because production deployment requires Resco licenses, backend configuration, sync setup, and security policies — none of which the AI handles. The 12-month target of 10 production deployments from 200 registrations (5% conversion) is optimistic given B2B freemium benchmarks.
   - *Mitigation*: Build a **guided deployment path** (see Solution section). After successful QR preview, offer automated production checklist + partner handoff option. Without this bridge, you'll have great demo metrics and zero revenue.

5. **🟡 LLM cost economics (MEDIUM)**: If users need 50+ AI turns per working app, the $70-100/month subscription may not cover LLM costs per user.
   - *Mitigation*: Track average turns-per-app in beta. Adjust credit pricing/included allowance based on real data. Tokenomics TBD — Requires validation.

6. **🟡 Team capacity vs. AI quality bar (MEDIUM)**: 2.5 FTE can build the MVP, but maintaining AI quality requires continuous prompt engineering, template refinement, model evaluation, and user feedback loops. Competitors have entire teams dedicated to this.
   - *Mitigation*: Budget for at least 1 dedicated FTE on AI quality/prompt engineering post-launch. This is the most important role in the team.

**Key unknowns**:
- Will new prospects (not existing Resco users) adopt this tool? — TBD - Core bet
- Turns-per-working-app (drives LLM cost economics) — TBD - Requires measurement
- Organic signup rate at vibe.resco.net — TBD - New channel, zero baseline
- Microsoft's timeline for vibe.powerapps.com offline improvements — TBD - External dependency (but moving fast)
- Salesforce MAGE feature roadmap and offline capabilities — TBD - New competitor, monitor closely
- Conversion rate from free credits to paid subscription — TBD - Requires validation

**Assumptions to validate**:
- ~10,000+ addressable firms across three ecosystems (research-based, not customer-validated)
- New prospects will use an AI code editor workflow (behavior assumption)
- MCP server provides sufficient context for first-try-accurate code generation (technically mature, user validation needed)
- Live preview via QR code is technically reliable across platforms
- 5 free credits is enough to build a convincing first app
- $70-100/month is acceptable pricing for this segment
- $10/user/month Resco license competes on value vs $10-20/user Power Apps (price parity, not advantage)
- RescoCloud sandbox works as frictionless demo backend
- 5-10% of entries convert to production deployments (stress-tested, was 20%)

---

## 🏁 Competitive Reality Check (as of Feb 2026)

| Capability | Resco Vibe Studio | Power Apps Vibe | Salesforce MAGE | Lovable | Bolt.new | v0 (Vercel) | Mendix |
|------------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **NL → full app** | 🔜 Planned | ✅ Live (preview) | ⚠️ Dev preview | ✅ Live | ✅ Live | ✅ Live | ⚠️ Partial |
| **Offline-first** | ✅ **Native** | ❌ Limited | ❌ SDK-level | ❌ No | ❌ No | ❌ No | ⚠️ React Native |
| **Multi-backend** | ✅ **D365+SF+SN** | ❌ MS only | ❌ SF only | ❌ Supabase | ❌ Various | ❌ Various | ✅ Any |
| **Price/user/month** | $10 | $10-20 | Varies | N/A (SaaS) | N/A (SaaS) | N/A (SaaS) | $50+ |
| **Field service focus** | ✅ **Core** | ⚠️ One of many | ⚠️ One of many | ❌ Generic | ❌ Generic | ❌ Generic | ⚠️ Horizontal |
| **Data encryption (local)** | ✅ Default | ❌ Not default | ⚠️ SF standard | N/A | N/A | N/A | ⚠️ Varies |
| **AI maturity** | ❌ Pre-MVP | ✅ Production | ⚠️ Preview | ✅ $200M ARR | ✅ Production | ✅ SOC 2 Type II | ✅ In prod |
| **Sync speed** | ✅ Up to 10x | ⚠️ Standard | ⚠️ Standard | N/A | N/A | N/A | ⚠️ Standard |

**Key insight**: Resco's competitive advantage is the intersection of three things — **offline-first + multi-backend + field-service-specific**. No single competitor matches all three. But Resco is also the **only one that hasn't shipped AI app generation yet**. Every month of delay narrows the competitive window.

**The race**: Microsoft and Salesforce are shipping AI now but lack offline/multi-backend. Lovable/Bolt/v0 have mature AI but lack enterprise field service. **Resco needs to ship its AI before Microsoft/Salesforce fix their offline gaps.**

---

## 🎬 Next Steps

**MONTH 1-2: Build MVP prototype**
- Dataverse + ServiceNow backend support
- UIReplacement generation via MCP server + Claude/LLM
- Monaco editor with iterative prompting
- QR-based live device preview
- RescoCloud sandbox for frictionless trial
- Registration + 5 free credits

**MONTH 2-3: Closed beta with 10-15 users**
- Mix of new prospects (primary — test the acquisition thesis) AND existing partners (secondary — test quick-solution use case)
- Each builds one real UIReplacement app
- **Measure**: time-to-first-app, AI accuracy, completion rate, NPS, license intent

**Decision criteria**:
- ✅ **10+ users complete a working app, time-to-first-app < 1 hour, > 3 express intent to deploy to production**: Proceed to open beta
- ⚠️ **5-9 complete, mixed feedback**: Identify friction (UX? AI quality? scope?), iterate, retest
- ❌ **< 5 complete or no production intent**: Reassess — pivot UX or scope

**MONTH 4-5**: Open beta (all partners + public waitlist)
**MONTH 6**: Public launch at vibe.resco.net
**MONTH 6-12**: Scale to 200 registrations, 40 paid, 10 production deployments

**Why this matters**: The entire bet is that **lowering the barrier to entry with AI will unlock the ~10,000 implementation firms** currently blocked by Woodford's learning curve. If a new prospect can go from "never heard of Resco" to "working app on my phone" in under an hour, Resco's addressable market expands dramatically. Validate this before investing in Phase 2 features.

---

## ⚠️ Reality Check

**This is a customer acquisition play with real strategic value and manageable cost.** At €185-285K Year 1 with 2.5 FTE, the investment is moderate. Under stress-tested assumptions, Year 1 revenue lands at €44-103K (not the original €153-363K). **Budget for a 2-year payback period, not 1 year.** The risk profile is still acceptable — the investment survives failure.

**Success depends on**:
1. AI code quality earning trust on first try with users who can't fix it manually
2. New prospects actually discovering and trying vibe.resco.net (requires marketing budget, not just organic)
3. Demo users converting to production deployments via guided deployment path (the North Star)
4. Staying ahead of Microsoft AND Salesforce before they close the offline/multi-backend gap (6-12 month window)

**If Microsoft closes the offline gap**: Go deeper on multi-backend (Salesforce, ServiceNow, Zoho, HubSpot — the one moat Microsoft will never cross) + expand Vibe Studio capabilities (AI agents, components, questionnaires).

**If Salesforce MAGE captures the SF segment**: Double down on the multi-backend value prop. MAGE only works with Salesforce. Resco works with SF + D365 + ServiceNow. Target multi-CRM organizations.

**If AI quality isn't good enough**: Ship templates with AI customization first (higher success rate). Invest in prompt engineering (1 dedicated FTE). MCP server provides the context layer — the gap is in generation quality, which is improvable.

**If new prospects don't convert**: Diagnose: discovery (need marketing budget), activation (UX/first-try quality), or value (tool doesn't solve real enough problem). Each has a different fix. The conversion funnel (see above) will reveal where users drop off.

**Remember**: "The only AI app builder that works offline, with any CRM backend." — If Vibe Studio delivers on this promise, it becomes Resco's primary growth engine. The multi-backend + offline-first + AI combination directly addresses why Resco loses deals today (complexity and platform lock-in perception).

---

**Created**: 2026-02-06 | **Updated**: 2026-02-08 (independent validation + challenge) | **Next Review**: 2026-03-06 | **Owner**: RESCO Product Team
