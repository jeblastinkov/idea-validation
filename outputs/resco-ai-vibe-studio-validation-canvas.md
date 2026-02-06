# Lean Canvas: RESCO AI Vibe Studio

**Date**: 2026-02-06 | **Company**: RESCO | **Version**: 2.0 | **Status**: Validated (Interactive Review)

---

## 📋 Executive Summary

**Idea**: AI-powered web studio (vibe.resco.net) that lets new prospects and business app makers build complete enterprise mobile apps through natural language — running inside Resco's proven offline-first mobile container with multi-backend support. "Build business apps when others fail."

**Target**: New prospects from MS Dynamics (~5,000 partners), Salesforce (~3,400 partners), and ServiceNow (~1,300 partners) ecosystems who need offline-first mobile apps but face high barriers to entry with current tools

**Economics**: €185-285K Year 1 (2.5 FTE + LLM + infra), hybrid revenue: $70-100/month Vibe Studio subscription + $10/user/month Resco license (primary). Moderate scenario: ~€363K Year 1 combined revenue. Break-even achievable in Year 1.

**Risk**: AI-generated code quality must earn trust on first try with users who can't fix it manually; Microsoft's vibe.powerapps.com may close the offline gap

**Next Action**: Build MVP (Month 1), closed beta with new prospects on real use cases (Month 2-3), measure time-to-first-app and Resco license conversion

---

## 🎯 Problem

### Top 3 Problems (Priority Order)
1. **High skill barrier blocks new customer acquisition**: Resco Woodford is proprietary and unique — every new prospect must invest significant time mastering it before they can build anything. This blocks growth. New partners/customers who are experienced in Microsoft, Salesforce, or ServiceNow stacks cannot easily adopt Resco. (Source: partner feedback, customer interviews, internal observations)
2. **Slow build-test-deploy cycle**: Even for those who can build, creating Resco mobile apps requires manual Woodford configuration + coding + sync + device testing — a cycle that takes hours-to-days per iteration with no live preview capability. (Source: partner feedback, experience)
3. **Competitors offer modern AI-assisted tooling**: vibe.powerapps.com and other platforms now offer AI-generated apps. Resco has no equivalent — risking perception as outdated among new prospects evaluating platforms

### Existing Alternatives
- **Woodford** (Resco's config tool): Powerful but steep learning curve, no live preview, requires deep expertise — works for existing partners, blocks new ones
- **Power Apps** ($20/user/month): AI-assisted, but Microsoft-only backend, limited offline, no native mobile experience out of the box
- **Salesforce Mobile SDK / ServiceNow Mobile Studio**: Platform-locked, offline-first remains a "pro-code effort" (Forrester)
- **Generic AI coding tools** (ChatGPT/Copilot): Hallucinate Resco APIs, no backend schema access, no device preview

---

## 👥 Customer Segments

**Primary**: New prospects — implementation partners and consultants experienced in Microsoft D365, Salesforce, or ServiceNow who need offline-first mobile app capabilities but don't know Resco Woodford. Vibe Studio is their **entry point** into the Resco ecosystem, skipping Woodford entirely.

**Secondary**: Existing Resco partners building quick, simple solutions (e.g., external user apps, simple data capture) — use cases that don't require robust workflows or deep Woodford expertise. For complex projects, existing partners use Woodford + MCP server.

**Market size**:
- **TAM**: ~10,000+ implementation firms (MS D365 ~5,000 + Salesforce ~3,400 + ServiceNow ~1,300) + tens of thousands of individual consultants | Field service market $5-9B growing 11-16% CAGR (Source: MarketsandMarkets, Mordor Intelligence, Alten Capital)
- **SAM**: Firms needing offline-first mobile — 60% of field workers need full offline access, only 30% of solutions deliver it (Source: Gartner, Forrester)
- **SOM (Year 1, moderate)**: ~140 new entries (5x current baseline of 28 new partners/customers per year)

**Reachability**: Resco partner account managers (16 active partners) | vibe.resco.net organic signups (new channel) | Microsoft Dynamics / Salesforce / ServiceNow LinkedIn groups and forums | Resco events and conferences

**Current acquisition baseline**: ~8 new partners/year + ~20 new customers/year = 28 new entry points (without Vibe Studio)

---

## 💎 Unique Value Proposition

**"Build business apps when others fail. Half the price of Power Apps."**

**Full statement**: "We help business app makers build enterprise mobile apps with AI — running inside Resco's proven offline-first container with multi-backend support and enterprise-grade security. No mobile infrastructure to build. No platform lock-in. No Woodford expertise needed."

**High-level concept**: "Like vibe.powerapps.com, but your app works offline, connects to any CRM backend, and costs half the price"

**Why different**:
- vs **Power Apps / vibe.powerapps.com**: Offline-first (proven by thousands of customers), multi-backend (not Microsoft-only), $10/user vs $20/user
- vs **Salesforce Mobile / ServiceNow Mobile**: Platform-agnostic — one app works with any backend, not locked to one ecosystem. Offline-first is easy, not a "pro-code effort"
- vs **Lovable / Bolt / v0**: Output runs in enterprise-grade Resco mobile container with security, sync, and offline — not a generic web app
- vs **Woodford**: AI-generated, no learning curve, live preview — accessible to newcomers who've never seen Woodford

**Why now**: "Vibe coding" trend + 60% offline demand vs 30% supply gap + Microsoft pushing AI-assisted development (vibe.powerapps.com) = market window for Resco to capture multi-backend offline-first position before competitors close the gap

---

## ✨ Solution

### Top 3 MVP Features (Phase 1 — UIReplacement, New Customer Acquisition)
1. **Frictionless onramp**: Register at vibe.resco.net → get 5 free credits → start immediately with RescoCloud sandbox (pre-configured demo backend, zero setup) OR connect own backend (Dataverse, Salesforce, ServiceNow) → create mobile project
2. **AI-powered full app generation**: Describe app in natural language → AI (Claude/LLM via Resco MCP server, pre-configured by Resco) generates complete UIReplacement code → displayed in Monaco editor with real-time progress → iterate with prompts or manual edits. User focuses on business logic — Resco container provides offline sync, security, and mobile experience automatically
3. **QR-based live device preview + publish**: Scan QR → app appears on physical device → auto-refreshes on code changes (live dev mode) → publish to production when ready, continue developing

### Delivery Channel
Web application at vibe.resco.net (browser-based, no local installation). AI/LLM provided by Resco's pre-configured environment (user does not bring own API key — credits cover AI costs).

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

**Platform owner moat**: Only Resco can build deeply integrated AI code generation for its own mobile container — proprietary access to Woodford metadata APIs, mobile project structure, offlinehtml deployment pipeline, sync infrastructure. Third parties cannot replicate this.

**Proven mobile container**: Thousands of business customers running Resco offline-first mobile apps in production. The generated code inherits enterprise-grade security, offline sync, and native mobile experience without the developer building any of it.

**Multi-backend (the Microsoft-proof moat)**: Resco works with Dataverse, Salesforce, ServiceNow, and more coming. Microsoft will never support non-Microsoft backends. This is the differentiator that survives even if Microsoft closes the offline gap.

**MCP server synergy**: Already in development — provides the AI context layer (JSBridge docs, backend schemas, sync analysis) that makes code generation accurate. Shared investment with separate initiative.

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

**Pricing advantage**: Resco $10/user/month vs Power Apps $20/user/month — 50% cost advantage, directly addressing the #1 reason Resco loses deals today

**Per-project revenue** (indirect): 20 users (avg) × $10/month × 24 months retention = $4,800 per project

**Investment** (2.5 FTE team):
- Build: 2.5 FTE × 6 months = €75-100K
- LLM API costs: €30-60K/year (scales with usage)
- Infrastructure: €30-50K/year (RescoCloud sandbox, hosting, preview)
- Maintenance (post-launch): €50-75K/year (same 2.5 FTE)
- **Total Year 1**: €185-285K

**Revenue forecast (Year 1)**:

| Stream | Conservative (10% deploy) | Moderate (20% deploy) |
|--------|--------------------------|----------------------|
| Direct (Vibe Studio subs) | ~€27K | ~€27K |
| Indirect (Resco licenses) | ~€126K | ~€336K |
| **Total** | **~€153K** | **~€363K** |

**Break-even**: Moderate scenario profitable in Year 1. Conservative scenario break-even early Year 2.

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

**Top 5 Risks**:

1. **AI code quality (HIGHEST)**: Generated UIReplacement code doesn't work reliably → new prospects (who can't debug Resco code) lose trust on first attempt and never return
   - *Mitigation*: MCP server is mature enough today (confirmed). Continuous iterative improvement on quality. Monaco editor allows manual fixes as fallback. Extensive testing before beta.

2. **vibe.powerapps.com competition (VERY HIGH)**: Microsoft expands AI app generation with improved offline and lower pricing → Resco's two main differentiators (offline-first, price) weaken
   - *Mitigation*: Speed to market. If Microsoft closes the gap: **go deeper on multi-backend** (the one thing Microsoft will never do) **+ expand Vibe Studio capabilities** (AI agents, components, questionnaires) to widen feature moat.

3. **New prospect conversion (HIGH)**: 5x growth assumption (28 → 140 entries/year) is unproven. Organic discovery at vibe.resco.net is a new channel with zero baseline data.
   - *Mitigation*: Track registration source from day 1. Invest in "build an app in 5 minutes" demo content. Leverage SF/SN community channels.

4. **Demo-to-production gap (MEDIUM)**: Users build cool demos with free credits but never deploy to production → $0 North Star revenue
   - *Mitigation*: Design onboarding flow that guides toward production deployment. Track funnel from registration → app created → app on device → production publish → license purchase.

5. **LLM cost economics (MEDIUM)**: If users need 50+ AI turns per working app, the $70-100/month subscription may not cover LLM costs per user
   - *Mitigation*: Track average turns-per-app in beta. Adjust credit pricing/included allowance based on real data. Tokenomics TBD — Requires validation.

**Key unknowns**:
- Will new prospects (not existing Resco users) adopt this tool? — TBD - Core bet
- Turns-per-working-app (drives LLM cost economics) — TBD - Requires measurement
- Organic signup rate at vibe.resco.net — TBD - New channel, zero baseline
- Microsoft's timeline for vibe.powerapps.com offline/multi-backend expansion — TBD - External dependency
- Conversion rate from free credits to paid subscription — TBD - Requires validation

**Assumptions to validate**:
- ~10,000+ addressable firms across three ecosystems (research-based, not customer-validated)
- New prospects will use an AI code editor workflow (behavior assumption)
- MCP server provides sufficient context for first-try-accurate code generation (technically mature, user validation needed)
- Live preview via QR code is technically reliable across platforms
- 5 free credits is enough to build a convincing first app
- $70-100/month is acceptable pricing for this segment
- $10/user/month Resco license wins against $20/user Power Apps
- RescoCloud sandbox works as frictionless demo backend
- 20% of entries convert to production deployments (moderate scenario)

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

**This is a customer acquisition play with real strategic value and manageable cost.** At €185-285K Year 1 with 2.5 FTE, the investment is moderate. The moderate revenue scenario (€363K) makes it profitable in Year 1. Even the conservative scenario (€153K) breaks even early Year 2. The risk profile is acceptable.

**Success depends on**:
1. AI code quality earning trust on first try with users who can't fix it manually
2. New prospects actually discovering and trying vibe.resco.net (organic channel is unproven)
3. Demo users converting to production deployments and Resco licenses (the North Star)
4. Staying ahead of Microsoft before they close the offline/multi-backend gap

**If Microsoft closes the offline gap**: Go deeper on multi-backend (Salesforce, ServiceNow, Zoho, HubSpot — the one moat Microsoft will never cross) + expand Vibe Studio capabilities (AI agents, components, questionnaires).

**If AI quality isn't good enough**: Continuously iterate. MCP server is mature — the gap is likely in prompt engineering and template quality, not infrastructure. This is improvable.

**If new prospects don't convert**: Consider whether the problem is discovery (marketing), activation (UX), or value (the tool doesn't solve a real enough problem). Each has a different fix.

**Remember**: "Build business apps when others fail. Half the price of Power Apps." — If Vibe Studio delivers on this promise, it becomes Resco's primary growth engine. The $10/user pricing + AI-assisted development directly addresses both reasons Resco loses deals today (price and complexity).

---

**Created**: 2026-02-06 | **Validated**: 2026-02-06 (interactive 8-skill review) | **Next Review**: 2026-03-06 | **Owner**: RESCO Product Team
