# Lean Canvas: Resco MCP Server

**Date**: 2026-01-21 | **Company**: RESCO | **Status**: Pre-Launch (1 week to MVP)

---

## 📋 Executive Summary

**Idea**: Free MCP server giving AI coding assistants direct access to Resco JSBridge docs + client Dataverse schemas, eliminating hallucinations when building Resco apps

**Target**: 15,000 senior functional consultants at Microsoft implementation partners globally who build Resco mobile apps monthly

**Economics**: €37.5K Year 1 investment (€22.5K build + €15K maintenance), break-even at 8 projects (~160 mobile end-users), expected 4-5 projects = -€13-18K Year 1 (acceptable), profitable Year 2-3

**Risk**: Consultants may not adopt (behavior change) + Microsoft/Resco likely building native solution (high competition risk) + no defensible moat

**Next Action**: Beta test with 15 consultants THIS WEEK (5 internal + 10 partners), need 10/15 regular usage to proceed with launch

---

## 🎯 Problem

**Top 3 Problems**:
1. AI coding assistants (Claude, Copilot, ChatGPT) hallucinate when generating Resco code due to missing JSBridge documentation context
2. Consultants waste hours manually searching Resco Wikipedia and troubleshooting sync issues
3. AI tools can't access client's Dataverse schema, forcing manual entity/field lookups and creating errors

**Current alternatives**: Manual Resco Wikipedia searches (slow, requires expertise) | ChatGPT with uploaded docs (incomplete, still hallucinates) | Hire developers for custom HTML (expensive) | Switch to Power Platform (lose Resco's offline-first advantages)

**Impact**: Significant time waste, implementation errors, steep learning curve, consultant frustration

---

## 👥 Customer Segments

**Primary**: Senior functional consultants at Microsoft Dynamics 365 implementation partners (100-250 employees) who build Resco mobile apps monthly per project

**Secondary**: In-house enterprise teams maintaining business applications on Microsoft ecosystem

**Market size**: ~15,000 consultants globally (3,000 MS partners × 175 avg employees × 30% consultants × 10% Resco users) | 16 active Resco partners (immediate reach) | Western Europe and US primarily

**Reachability**: Resco partner network (16 partners, 80 potential early users) | Microsoft Copilot Studio marketplace | MS Dynamics LinkedIn groups/forums | Resco documentation integration

---

## 💎 Unique Value Proposition

**"We help functional consultants build Resco apps 10x faster by giving AI assistants direct access to Resco docs and their Dataverse schema—eliminating hallucinations and manual lookups."**

**High-level concept**: "Like GitHub Copilot, but it actually knows Resco JSBridge and your specific Dataverse structure"

**Why different**:
- vs Manual ChatGPT: Direct live Dataverse connection + full Resco docs (zero hallucination)
- vs vibe.powerapps.com: Only solution for Resco ecosystem (not Power Apps)
- vs Manual search: Automatic context in AI workflow (no context switching)

---

## ✨ Solution

**MVP (3 tools)**:
1. **Resco JSBridge documentation search**: AI-accessible Resco Wikipedia, eliminating hallucinations
2. **Dataverse schema access**: List entities/tables/fields from client's Dynamics org for accurate code generation
3. **Sync log analysis**: Troubleshoot Resco mobile app synchronization issues with AI

**Delivery**: Model Context Protocol (MCP) server compatible with Claude, Microsoft Copilot Studio, other MCP tools

**Distribution**: Published to Microsoft Copilot Studio marketplace for one-click installation

**NOT in MVP**: Workflow builder (#4) | Code templates | Multi-org management | Usage analytics | Mobile preview | Code review

---

## 🔑 Unfair Advantage

**First-mover**: Only MCP server for Resco development, leveraging Resco's unique positioning (offline-first mobile vs Power Platform online-first | platform-agnostic: Dataverse + Salesforce + ServiceNow | native mobile performance)

**Distribution**: Direct Microsoft Copilot Studio marketplace access + established 16-partner network

**Speed**: 1 week to launch, establishing category before Microsoft/Resco builds native solution

**Reality check**: Easily replicable, no tech moat—advantage is speed only

---

## 📊 Channels

**Primary**: Microsoft Copilot Studio marketplace (organic discovery)

**Early adopters**: 16 Resco partners → Beta with 5 internal + 10 partner consultants

**Community**: MS Dynamics LinkedIn groups | Forums (Reddit r/Dynamics365) | Resco documentation integration | Conferences (Dynamics 365, Resco events)

**Launch strategy**: Week 1-2 beta testing → Week 3 marketplace launch → Week 4+ community engagement + partner webinars

**Viral loop**: Consultants share AI-assisted code with colleagues → organic spread within partner firms

---

## 💰 Economics

**Revenue model**: Free MCP server drives Resco mobile app licenses (€10/user/month) sold by partners to end customers

**Business logic**: Free tool → More consultants can build Resco apps → More projects delivered → More licenses sold

**Per-project revenue**: 20 users (avg) × €10/month × 24 months retention = €4,800

**Investment**:
- Build: 1.5 FTE × 3 months = €22,500 (€60K/year dev cost)
- Maintenance: €15,000/year
- **Year 1 total**: €37,500

**Break-even**:
- Year 1: €37,500 / €240 per user = 156 users = ~8 projects
- Year 2+: €15,000 / €240 = 63 users = ~3 projects/year

**Forecast**: 4-5 projects Year 1 (conservative) = 80-100 users = €19-24K revenue = **-€13-18K net** (acceptable investment)

**Profitability**: Year 2-3 as adoption scales to 11+ projects/year

---

## 📈 Key Metrics

**North Star**: Active users (unique consultants using MCP monthly)

**Success criteria**:
- 6 months: 20 active users
- 12 months: 50+ active users

**Supporting metrics**:
- MCP connections/tool uses: 500+ in 6 months (25 uses per user = engagement depth)
- Time reduction: 10x faster (target, unvalidated)
- Projects delivered with MCP: 8+ in Year 1
- Mobile end-users on MCP-built UIs: 156+ Year 1 (break-even)

**Tracking**: MCP server logs (anonymous analytics) | Partner surveys (quarterly) | Consultant interviews | Resco license correlation

---

## 🚨 Critical Risks

**Riskiest assumption**: Consultants will actually adopt and use MCP in daily workflow (requires behavior change + AI trust + learning curve + time investment)

**Top 5 Risks**:

1. **Adoption (HIGHEST)**: Consultants don't use MCP → Zero ROI, €37.5K wasted
   - *Mitigation*: Pre-launch beta with 15 consultants, need 10/15 regular usage

2. **Competition (VERY HIGH)**: Microsoft/Resco builds native MCP before/after launch → First-mover advantage eliminated
   - *Likelihood*: Very high (acknowledged)
   - *Mitigation*: Speed to market (1 week), potential partnership pivot

3. **No moat**: Easily replicable technology → Commoditized quickly
   - *Mitigation*: None beyond speed

4. **Value (MEDIUM)**: Time savings <5x → Insufficient to change behavior
   - *Mitigation*: Measure in beta, adjust expectations

5. **Distribution (MEDIUM)**: Copilot Studio approval delayed/rejected → Limited reach
   - *Mitigation*: Claude/other MCP tools as backup

**Key unknowns**: 10x speed claim unvalidated | Viral coefficient unknown | MS/Resco timeline unclear | Consultant authority to adopt tools | Retention beyond trial

**Assumptions to validate**:
- 15K market size (estimated, not confirmed)
- 20 users/project (varies by type)
- 24-month retention (industry avg)
- 4-5 projects Year 1 (conservative guess)
- Consultants have tool adoption authority

---

## 🎬 Next Steps

**THIS WEEK: Beta validation with 15 consultants**

**Setup**:
- Recruit: 5 internal Resco + 10 from partner firms
- Demo: Hands-on MCP setup + integration
- Test: Real project work (build Resco offline HTML for actual client)
- Observe: 1 week usage

**Measure**:
- How many use it? (target: 10/15)
- How often? (daily/weekly/never)
- Time savings? (really 10x or less?)
- Code accuracy? (hallucination reduction)
- Would recommend? (viral potential)

**Decision criteria**:
- ✅ **10+ regular users**: Launch to Copilot Studio marketplace Week 3
- ⚠️ **5-9 users**: Identify friction, iterate, retest
- ❌ **<5 users**: Stop or major pivot (adoption risk too high)

**Timeline**:
- Week 1-2: Beta testing
- Week 2 end: Go/no-go decision
- Week 3: Copilot Studio launch (if validated)
- Month 3: 20 active users target
- Month 6: 8+ projects target

**Why this matters**: If consultants won't use it when free + actively supported, they won't use it at scale. Validate adoption BEFORE broader distribution.

---

## 📝 Key Assumptions

- 15K addressable market (estimation, not validated data)
- 10x faster development (marketing claim, requires measurement)
- Consultants will integrate AI into workflow (behavior change required)
- 20 users per project average (varies by project type)
- 24-month customer retention (industry benchmark, not Resco-specific)
- 4-5 new projects in Year 1 (conservative estimate, unvalidated)
- Microsoft Copilot Studio will approve listing (assumed)
- Code accuracy from MCP is acceptable (>70% correct)
- Consultants have authority to adopt new tools (may need approval)
- Viral spread within partner firms (organic growth assumption)

*Mark all unknowns as "TBD - Requires validation"*

---

## ⚠️ Reality Check

**This is a speed play, not a moat play.** Competitive advantage is launching first (1 week) before Microsoft/Resco builds native solution. MCP itself is easily replicable—no defensible technology or network effect.

**Success depends on**:
1. Consultants actually adopt (10/15 in beta)
2. Fast viral spread (20 users in 6 months from 16 partners)
3. Converting usage to projects (8+ Year 1)
4. Microsoft/Resco delay native solution (uncertain, likely short window)

**If Microsoft/Resco announce native MCP**: Pivot to partnership (contribute MCP to become official) rather than compete.

**Risk-adjusted approach**: Proceed with 1-week launch (low cost, fast validation) → Test aggressively → Decide on real data → Stay flexible for partnership pivot

**Remember**: Goal is driving Resco license sales, not building standalone product. Even if commoditized, you win if it accelerates Resco adoption in the meantime.

---

**Created**: 2026-01-21 | **Next Review**: 2026-02-04 (post-beta) | **Owner**: RESCO Product Team
