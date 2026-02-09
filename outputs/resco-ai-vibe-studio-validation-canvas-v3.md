# Lean Canvas: RESCO AI Vibe Studio

**Date**: 2026-02-08 | **Version**: 3.0 | **Status**: Validated + Challenged

---

## Executive Summary

**What**: AI web studio (vibe.resco.net) — build enterprise mobile apps via natural language, running in Resco's offline-first container with multi-backend support.

**Who**: New prospects from MS Dynamics (~5K partners), Salesforce (~3.4K partners), ServiceNow (~1.3K partners) who need offline mobile but face high entry barriers.

**Cost**: €185-285K Year 1 (2.5 FTE + LLM + infra). Revenue: $70-100/month subscription + $10/user/month Resco license. Stress-tested Year 1: €44-103K. Break-even Year 2.

**Key risks**: AI code must work on first try for users who can't fix it | vibe.powerapps.com already live | Salesforce MAGE launched Feb 2026.

**Next action**: Build MVP (Month 1), closed beta with new prospects (Month 2-3), measure time-to-first-app and license conversion.

**Verdict**: Sound strategy, manageable cost. Budget for 2-year payback. The multi-backend + offline-first moat is real — but ship fast.

---

## Problem

1. **Skill barrier blocks growth**: Resco Woodford requires deep expertise — blocks new prospects from MS/SF/SN ecosystems
2. **Slow build cycle**: Manual config + coding + sync + device testing = hours-to-days per iteration, no live preview
3. **Competitors ship AI tooling**: vibe.powerapps.com and SF MAGE are live — Resco risks looking outdated

**Alternatives**: Woodford (powerful but steep) | Power Apps ($10-20/user, limited offline) | SF MAGE (SF-only) | Lovable/Bolt/v0 (no enterprise offline/CRM) | Generic AI tools (hallucinate Resco APIs)

---

## Customer

**Primary**: New prospects — partners/consultants from D365, Salesforce, ServiceNow who need offline mobile but don't know Woodford. Vibe Studio is their entry point.

**Secondary**: Existing Resco partners for quick, simple solutions.

**Market**: ~10,000+ implementation firms (D365 ~5K + SF ~3.4K + SN ~1.3K). Low-code market ~$45-52B, 19% CAGR. Field service $5-9B, 11-16% CAGR.

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

To reach 10 deployments: need ~6,000 visitors. Requires active marketing — organic alone won't suffice.

---

## Value Proposition

**"The only AI app builder that works offline, with any CRM backend."**

**High-level**: "Like vibe.powerapps.com, but works offline and connects to any CRM — not just Microsoft."

| vs | Resco advantage |
|----|-----------------|
| Power Apps / vibe.powerapps.com | Offline-first + encrypted data + multi-backend. PA: no offline flows, no default encryption |
| Salesforce MAGE | Platform-agnostic vs SF-only |
| Lovable / Bolt / v0 | Enterprise container with security, sync, offline — not a generic web app |
| Woodford | AI-generated, no learning curve, live preview |

**Window**: 6-12 months before MS/SF close the offline gap.

---

## Solution (MVP)

1. **Frictionless onramp**: Register at vibe.resco.net → 5 free credits → RescoCloud sandbox (zero setup) or connect own backend
2. **AI full app generation**: Natural language → complete UIReplacement code via MCP + LLM → Monaco editor → iterate with prompts or manual edits
3. **QR live preview + publish**: Scan QR → app on device → auto-refresh on changes → publish when ready

### Critical MVP additions

**Guided deployment wizard** (addresses #1 revenue risk — demo-to-production gap):
- "Ready to deploy?" after successful preview
- Automated checklist: backend, sync, security, licenses
- Partner handoff option for assisted deployment

**Template library** (higher first-try success than freeform):
- 5-10 templates: field inspection, work orders, inventory, sales visits, delivery/proof
- User customizes via AI prompts on working baseline

**NOT in MVP**: Form Components | AI Assistants | Questionnaire builder | List Components | Marketplace | Multi-user collab | Additional backends (Year 2-3)

---

## Unfair Advantage

**Three capabilities no competitor matches:**

| | Resco | Power Apps | SF MAGE | Lovable | Mendix |
|---|:---:|:---:|:---:|:---:|:---:|
| Offline-first (native) | **Yes** | Limited | SDK-level | No | Partial |
| Multi-backend (D365+SF+SN) | **Yes** | MS only | SF only | No | Yes |
| Field service specialized | **Yes** | Generic | Generic | No | Horizontal |
| AI app generation | Pre-MVP | Live | Preview | $200M ARR | In prod |

**Platform owner moat**: Only Resco can deeply integrate AI generation with its mobile container — proprietary Woodford APIs, deployment pipeline, sync infrastructure. Can't be replicated by third parties.

**Multi-backend moat**: Microsoft will never support SF/SN. Salesforce will never support D365. This survives even if both fix offline.

**MCP synergy**: Already in development — shared investment, dual benefit.

**Weakness**: Only major player that hasn't shipped AI generation yet. Every month of delay narrows the window.

---

## Channels

**Primary**: vibe.resco.net organic signups (5 free credits) + partner account managers

**Launch**: Month 1-2 build → Month 2-3 closed beta (10-15 users) → Month 4-5 open beta → Month 6 public launch

**Viral loop**: Free credits → working app → demo to client → production need → license sale → peer recommendation

---

## Economics

**Revenue**: Hybrid — Vibe Studio subscription ($70-100/month, credit-based) + Resco licenses ($10/user/month, North Star).

**Per-project** (indirect): 20 users × $10/month × 24 months = $4,800

**Investment**:

| Item | Amount |
|------|--------|
| Build (2.5 FTE × 6 months) | €75-100K |
| LLM API costs | €30-60K/year |
| Infrastructure | €30-50K/year |
| Maintenance (post-launch) | €50-75K/year |
| **Year 1 total** | **€185-285K** |

**Revenue forecast (Year 1)**:

| Scenario | Entries | Deploy rate | Revenue |
|----------|---------|-------------|---------|
| Stress-tested realistic | 42-84 (2-3x) | 5-10% | **€44-103K** |
| Original moderate | 140 (5x) | 20% | €363K |

**Break-even shifts to Year 2-3 under realistic assumptions.** Budget for 2-year payback.

---

## Key Metrics

**North Star**: Resco license revenue attributable to Vibe Studio users.

| Target | 6 months | 12 months |
|--------|----------|-----------|
| Registrations | 50 | 200 |
| Active users | 15 | 40 paid |
| Time-to-first-app | < 1 hour | < 1 hour |
| Production deployments | — | 10 |
| Attributable license ARR | — | $24,000 |

**Failure signals**: < 20 registrations at 6 months | time-to-first-app > 2 hours | < 5 deployments at 12 months | $0 attributable license revenue

---

## Critical Risks

| # | Risk | Severity | Core issue |
|---|------|----------|------------|
| 1 | **AI first-try quality** | HIGHEST | Non-experts can't debug failures. 70% success = 30% permanent churn. Lovable spent hundreds of millions here; we have 2.5 FTE. |
| 2 | **Competition** | VERY HIGH | vibe.powerapps.com live + expanding. SF MAGE launched Feb 2026. Both targeting same segments. |
| 3 | **Funnel reality** | HIGH | 5x growth assumption unsupported. Need ~6K visitors for 10 deployments. Requires marketing budget ($20-50K). |
| 4 | **Demo-to-prod gap** | HIGH | Every vibe tool struggles here. Resco's gap is worse: licenses + backend + sync + security needed. Without guided deployment = $0 revenue. |
| 5 | **LLM costs** | MEDIUM | If 50+ turns per app, subscription may not cover costs. Measure in beta. |
| 6 | **Team capacity** | MEDIUM | 2.5 FTE builds MVP but AI quality requires continuous prompt engineering. Budget 1 dedicated FTE post-launch. |

**Unvalidated**: New prospect adoption | turns-per-app | organic signup rate | MS/SF timelines | free-to-paid conversion | 5 credits sufficiency | $70-100/month pricing acceptance

---

## Next Steps

**Month 1-2**: Build MVP (Dataverse + SN support, UIReplacement gen, Monaco editor, QR preview, RescoCloud sandbox, registration + credits)

**Month 2-3**: Closed beta with 10-15 users (mix of new prospects + existing partners)

| Result | Action |
|--------|--------|
| 10+ complete app, < 1hr, 3+ intent to deploy | Proceed to open beta |
| 5-9 complete, mixed feedback | Identify friction, iterate, retest |
| < 5 complete or no deploy intent | Reassess — pivot UX or scope |

**Month 4-5**: Open beta | **Month 6**: Public launch | **Month 6-12**: Scale to 200 reg, 40 paid, 10 deployments

---

## Contingencies

| If... | Then... |
|-------|---------|
| MS closes offline gap | Go deeper on multi-backend (SF, SN, Zoho, HubSpot) + expand Vibe capabilities |
| SF MAGE captures SF segment | Double down on multi-backend — MAGE is SF-only |
| AI quality insufficient | Ship templates + AI customization first. Invest in prompt engineering (1 FTE) |
| New prospects don't convert | Diagnose: discovery (marketing) vs activation (UX) vs value (product). Funnel reveals where. |

---

**Bottom line**: €185-285K bet on customer acquisition. Multi-backend + offline-first is a real moat. Ship before MS/SF close the gap. Budget 2 years to break even. The core bet: if a new prospect can go from "never heard of Resco" to "working app on phone" in under an hour, the addressable market expands dramatically.

---

*Created: 2026-02-06 | Updated: 2026-02-09 (condensed executive version) | Next Review: 2026-03-06 | Owner: RESCO Product Team*
