# Lean Canvas: RESCO AI Vibe Studio

**Date**: 2026-02-10 | **Version**: 4.0 | **Status**: Validated + Competitively Challenged + Scope Narrowed

---

## Executive Summary

**What**: AI web studio (vibe.resco.net) that generates offline-first mobile field apps from natural language — running instantly in Resco's proven mobile container with any CRM backend. No compilation. No app store. Describe → generate → on your phone in minutes.

**Who**: Implementation partners and consultants from D365 (~5K partners), Salesforce (~3.4K), ServiceNow (~1.3K) who need offline mobile field apps but face high barriers with every platform's native tooling.

**Cost**: €185-285K Year 1 (2.5 FTE + LLM + infra). Revenue: $10/user/month Resco license (primary) + studio subscription TBD. Stress-tested Year 1: €44-103K. Break-even Year 2.

**Key risk**: AI code must work on first try for non-experts who can't debug | All three platform vendors (MS, SF, SN) are shipping their own AI builders — but all are locked to their own ecosystem and weak on offline.

**Next action**: Build MVP (Month 1-2), closed beta with field service prospects (Month 2-3), measure time-to-first-app and license conversion.

---

## Problem

1. **Every platform vendor locks you in**: Power Apps Vibe = Microsoft only. Agentforce Vibes = Salesforce only. Creator Studio = ServiceNow only. If your clients use multiple CRMs, you need multiple tools.
2. **Offline is still broken everywhere**: Power Apps adding "offline by default" (2026, untested). ServiceNow MAB has zero offline support. Salesforce requires custom SmartStore SDK development. No platform delivers turnkey offline for field work.
3. **Native mobile = compilation hell**: Salesforce MAGE generates Swift/Kotlin scaffolds you must compile yourself. Power Apps requires its own runtime. ServiceNow is web-only. None deliver "describe it → it's on your phone" without a build step.

**Alternatives today**:
| Alternative | What's wrong |
|-------------|-------------|
| Power Apps Vibe | MS-only. Offline "coming soon." Locked to Dataverse. |
| Agentforce Vibes + MAGE | SF-only. MAGE = scaffold only, you still code the app. SmartStore = manual dev. |
| SN Creator Studio + Build Agent | SN-only. Mobile App Builder has NO offline. Web apps only. |
| Lovable / Bolt / v0 | Generic web apps. No CRM, no offline, no field service. |
| Resco Woodford (current) | Powerful but steep learning curve, no AI, no live preview. Blocks new prospects. |

---

## Customer

**Primary**: Implementation partners and consultants experienced in D365, Salesforce, or ServiceNow who are asked to deliver offline mobile field apps. Today they either use platform-native tools (limited offline, locked to one CRM) or tell the client it can't be done.

**Secondary**: Existing Resco partners building quick solutions — field inspection forms, simple data capture apps — that don't need deep Woodford expertise.

**Market**: ~10,000+ implementation firms globally. Field service mobile market $5-9B, 11-16% CAGR. 60%+ of field service orgs plan mobile apps within 3 years (Gartner), yet none of the three major platforms deliver turnkey offline.

**Reachability**: Resco partner account managers (16 active) | vibe.resco.net organic signups | D365/SF/SN LinkedIn communities | Resco events

**Current baseline**: ~28 new entries/year without Vibe Studio.

### Year 1 Conversion Funnel

| Step | Conservative | Moderate |
|------|-------------|----------|
| Website visitors | 3,000 | 6,000 |
| Register (7%) | 210 | 420 |
| Build app (30%) | 63 | 126 |
| Test on device (50%) | 32 | 63 |
| Deploy to prod (20%) | 6 | 13 |
| Buy licenses (80%) | 5 | 10 |

Requires active marketing ($20-50K). Organic alone won't drive 6K visitors to a niche B2B tool.

---

## Value Proposition

**"AI-powered offline field apps. Any CRM. Minutes, not months."**

This is NOT "like Power Apps Vibe but better." This is the tool for the use case no platform vendor solves: **offline field apps that work across CRM ecosystems.**

### Why different — the 4 things no competitor matches together:

| | Resco | Power Apps Vibe | SF Agentforce + MAGE | SN Creator Studio |
|---|:---:|:---:|:---:|:---:|
| Turnkey offline (zero config) | **Yes** | Coming (2026) | No (manual SDK) | **No** (MAB has zero offline) |
| Multi-backend (D365+SF+SN) | **Yes** | MS only | SF only | SN only |
| No-compile deployment | **Yes** (runs in container) | PA runtime | **No** (Xcode/AS build required) | SN platform only |
| Field service specialized | **Yes** (18 years, 2,500 customers) | Generic | Generic | Generic |

**The no-compile advantage explained**: With Salesforce MAGE, AI generates a project skeleton — but you still open Xcode, configure signing certificates, compile for iOS, and submit to App Store. With Resco, the user describes the app, AI generates the code, user scans a QR code, and it runs inside the existing Resco app. No Xcode. No compilation. No app store. This is the fastest path from idea to phone.

**Window**: 3-6 months. MS adding "offline by default." SF iterating on MAGE. SN added Build Agent Dec 2025. All shipping fast — but all locked to their own ecosystem.

---

## Solution (MVP) — Focused on Field Apps Only

### Scope: UIReplacement apps for field service use cases. Nothing else.

1. **Frictionless onramp**: Register at vibe.resco.net → free credits → RescoCloud sandbox (zero setup) or connect own D365/SF/SN backend
2. **Template-first AI generation**: Choose from 5-10 field service templates → customize via natural language prompts → AI refines working baseline. Freeform NL generation available but templates are the primary path (higher first-try success rate, learned from SF MAGE's "factory model")
3. **QR instant preview + publish**: Scan QR → working app on phone → auto-refreshes on code changes → publish to production when ready. No build step.

### Field service templates (launch set):
- Work order management
- Field inspection form
- Asset check / inventory
- Delivery / proof of delivery
- Field sales visit report
- Property inspection

### Guided deployment path (critical for revenue):
- "Ready to deploy?" prompt after successful QR preview
- Automated checklist: backend verified → sync configured → security applied → license explained
- Partner handoff option for assisted deployment

### NOT in scope — CUT entirely:
| Cut feature | Reason |
|-------------|--------|
| AI Assistants / AI Pantheon | Platform feature — MS/SF/SN do this better with more resources. Dilutes focus. |
| Questionnaire builder | Niche within niche. No evidence of demand from new prospects. |
| Form Components (IFrame) | Existing-partner feature, not new-prospect acquisition driver. Revisit only if 10+ beta users request. |
| List Components | Undefined scope. Not needed for field service templates. |
| Marketplace for tools/snippets | Platform play. Resco is not a platform — it's a focused tool. |
| Multi-user collaboration | Enterprise feature. Premature for MVP validation. |

### Deferred to Phase 2 (only if Phase 1 validates):
- Form Components — if 10+ beta users request
- Additional backends (Zoho, HubSpot) — only if multi-backend proven as acquisition driver
- Component library expansion — based on actual usage data

---

## Unfair Advantage

**The intersection of four capabilities no competitor matches:**

1. **Turnkey offline** (18 years, 2,500 customers, encrypted, automatic sync) — no config by the developer
2. **Multi-backend** (D365 + Salesforce + ServiceNow) — Microsoft will never support SF. Salesforce will never support D365. ServiceNow will never support either.
3. **No-compile deployment** — QR scan → app on phone. No Xcode, no Android Studio, no app store.
4. **Field service depth** — 700+ mobile features specialized for field operations

**Platform owner moat**: Only Resco can integrate AI generation with its own container — proprietary Woodford APIs, offlinehtml pipeline, sync infrastructure. Third parties cannot replicate.

**MCP server synergy**: Resco MCP server (separate product, free) provides the AI context layer — JSBridge docs, backend schemas, sync analysis. Works as standalone addon for Claude/Cursor/Copilot AND powers Vibe Studio's code generation. Separate distribution, shared investment.

---

## MCP Server Relationship (Separate Product)

The Resco MCP server is a **separate, free product** — not part of Vibe Studio. It serves two audiences independently:

| | Resco MCP Server | Resco Vibe Studio |
|---|---|---|
| **What** | AI context layer (JSBridge docs, schemas, sync) | AI app generation studio |
| **For** | Existing consultants using their own IDE (Claude, Cursor, Copilot) | New prospects who don't know Resco |
| **How** | MCP tools in any MCP-compatible AI tool | Web app at vibe.resco.net |
| **Price** | Free | Credits + subscription |
| **Goal** | Accelerate existing partners, compete with SF DX MCP (60+ tools) | Acquire new customers |
| **Shared** | Same AI context data, same JSBridge docs, same schema access | Same AI context data, same JSBridge docs, same schema access |

**Why separate**: MCP server is an addon to 3rd-party AI tools — consultants choose their own IDE. This is a different value prop ("make your existing AI tools Resco-aware") vs Vibe Studio ("build Resco apps without knowing Resco"). Bundling them confuses both messages.

---

## Channels

**Primary**: vibe.resco.net organic signups (free credits) + Resco partner account managers

**Early adopters**: Field service consultants at D365 partners (Resco's home turf — start where you're strongest)

**Launch**: Month 1-2 build MVP → Month 2-3 closed beta (10-15 users, field service focus) → Month 4-5 open beta → Month 6 public launch

**Viral loop**: Free credits → working field app → demo to client on actual phone → client needs production → Resco license sale → consultant recommends to peers

---

## Economics

**Revenue model**: Resco licenses ($10/user/month) are the North Star. Studio subscription pricing TBD — consider free or low-cost to maximize adoption, since platform vendors offer free AI builders.

**Per-project** (indirect): 20 users x $10/month x 24 months = $4,800

**Investment**:

| Item | Amount |
|------|--------|
| Build (2.5 FTE x 6 months) | €75-100K |
| LLM API costs | €30-60K/year |
| Infrastructure | €30-50K/year |
| Maintenance (post-launch) | €50-75K/year |
| **Year 1 total** | **€185-285K** |

**Revenue forecast (Year 1)**:

| Scenario | Entries | Deploy rate | Revenue |
|----------|---------|-------------|---------|
| Stress-tested realistic | 42-84 (2-3x) | 5-10% | **€44-103K** |
| Original moderate | 140 (5x) | 20% | €363K |

**Pricing pressure**: Agentforce Vibes is free (50 req/day). SN Build Agent trial is free (25 calls). Power Apps Vibe is included in license. Charging $70-100/month for Vibe Studio creates friction when competitors give their builder away. **Recommendation**: Price for adoption — free or $30/month. Monetize on Resco licenses, not studio subscription.

**Break-even**: Year 2-3 under realistic assumptions. Budget for 2-year payback.

---

## Key Metrics

**North Star**: Resco license revenue attributable to Vibe Studio users.

| Target | 6 months | 12 months |
|--------|----------|-----------|
| Registrations | 50 | 200 |
| Active users | 15 | 40 paid |
| Time-to-first-app | < 30 min | < 30 min |
| Template usage rate | > 60% | > 60% |
| Production deployments | — | 10 |
| Attributable license ARR | — | $24,000 |

**Failure signals**: < 20 registrations at 6 months | time-to-first-app > 1 hour | < 5 deployments at 12 months | $0 attributable license revenue

---

## Critical Risks

| # | Risk | Severity | Core issue |
|---|------|----------|------------|
| 1 | **AI first-try quality** | HIGHEST | Non-experts can't debug. Template-first approach mitigates (deterministic base + AI customization), but freeform generation remains risky. Budget 1 FTE on prompt engineering post-launch. |
| 2 | **Competition speed** | VERY HIGH | MS/SF/SN all shipping AI builders now. All ecosystem-locked, all weak on offline — but improving fast. Ship MVP in 3 months. |
| 3 | **Pricing vs free competitors** | HIGH | SF Vibes: free. SN Build Agent: free trial. PA Vibe: included. Resco charging $70-100/month = adoption friction. Price for adoption, not profit. |
| 4 | **Demo-to-prod gap** | HIGH | Guided deployment path is critical. Without it: great demos, zero revenue. |
| 5 | **Funnel reality** | HIGH | Need ~6K visitors for 10 deployments. Requires $20-50K marketing budget. |
| 6 | **SF segment harder than assumed** | MEDIUM | Agentforce Vibes (60+ MCP tools, free) + MAGE + SmartStore = SF partners start there. Deprioritize SF, focus on D365 + SN. |

**Unvalidated**: New prospect adoption | turns-per-app | organic signup rate | template-vs-freeform usage split | pricing acceptance | MS offline timeline

---

## Next Steps

**Month 1-2**: Build MVP — template-first field app generation, QR preview, RescoCloud sandbox, D365 + SN backend support, registration + credits

**Month 2-3**: Closed beta with 10-15 field service users (mix of new D365/SN prospects + existing partners). Each builds one real field app from a template.

| Result | Action |
|--------|--------|
| 10+ complete app, < 30min, 3+ intend to deploy | Proceed to open beta |
| 5-9 complete, mixed feedback | Identify friction, iterate, retest |
| < 5 complete or no deploy intent | Reassess scope or pivot |

**Month 4-5**: Open beta | **Month 6**: Public launch | **Month 6-12**: 200 registrations, 40 paid, 10 deployments

---

## Contingencies

| If... | Then... |
|-------|---------|
| MS closes offline gap | Double down on multi-backend — the moat MS will never cross |
| SF MAGE evolves to full app builder | Lead with "no compile" + multi-backend. MAGE still requires Xcode/AS. |
| SN adds offline to MAB | Unlikely near-term (not on roadmap). If it happens, multi-backend remains. |
| AI quality insufficient | Template-first approach already mitigates. Invest in prompt engineering (1 FTE). |
| New prospects don't convert | Diagnose via funnel: discovery vs activation vs value. Each has a different fix. |
| Pricing resistance | Drop to free. Revenue = Resco licenses only ($10/user/month). |

---

**Bottom line**: Every platform vendor is building AI app generation for their own ecosystem. Resco cannot out-platform them. But Resco occupies an intersection none of them can reach: **turnkey offline + multi-backend + no-compile deployment + field service depth.** Win by staying narrow, shipping fast, and pricing for adoption. The core bet: a new prospect goes from "never heard of Resco" to "working offline field app on my phone" in under 30 minutes.

---

*Created: 2026-02-06 | Updated: 2026-02-10 (v4: scope narrowed, competitive challenge, pricing adjusted) | Next Review: 2026-03-10 | Owner: RESCO Product Team*
