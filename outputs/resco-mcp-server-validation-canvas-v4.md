# Lean Canvas: Resco MCP Server

**Date**: 2026-02-08 | **Version**: 4.1 | **Status**: Pre-Launch — Updated for Full Toolset

---

## Executive Summary

**What**: Free MCP server giving AI coding assistants 63 tools to read, build, and configure Resco Mobile CRM projects — forms, views, workflows, sync filters, home screen navigation, offline HTML files, and more. Eliminates hallucinations and replaces manual clicking in Woodford.

**Who**: ~15,000 senior functional consultants at MS implementation partners globally.

**Cost**: €37.5K Year 1 (€22.5K build + €15K maintenance). Break-even at 8 projects (~160 users). Expected Year 1: 4-5 projects = -€13-18K (acceptable). Profitable Year 2-3.

**Key risk**: Adoption (behavior change) + Microsoft/Resco likely building native solution + no defensible moat.

**Next action**: Beta with 15 consultants THIS WEEK. Need 10/15 regular usage to proceed.

**Verdict**: STRONG — Low risk, high strategic value. Even partial adoption pays for itself. Builds essential infrastructure for Vibe Studio.

---

## Problem

1. AI assistants hallucinate Resco code — missing JSBridge docs and platform awareness
2. Consultants waste hours clicking through Woodford UI to configure forms, views, workflows, and navigation
3. AI tools can't access client Dataverse schemas or live project structure — manual lookups, frequent errors
4. Sync troubleshooting is slow and opaque without AI-assisted log analysis

**Alternatives**: Manual wiki search (slow) | ChatGPT + uploaded docs (still hallucinates) | Hire devs (expensive) | Switch to Power Platform (lose offline-first)

---

## Customer

**Primary**: Senior functional consultants at MS D365 partners (100-250 employees), building Resco mobile apps monthly.

**Market**: ~15,000 consultants globally. 16 active Resco partners (80 potential early users). Western Europe + US.

**Reach**: Resco partner network | MS Copilot Studio marketplace | LinkedIn groups/forums

---

## Value Proposition

**"AI that doesn't just know Resco — it builds your entire app for you."**

- vs Manual ChatGPT: Live project connection + full docs + 63 tools = zero hallucination + actual configuration
- vs vibe.powerapps.com: Only complete AI-driven configuration solution for the Resco ecosystem
- vs Manual Woodford clicks: Describe what you want in plain language; AI configures forms, views, workflows, and navigation directly
- vs Manual search: Automatic AI context across the full Resco surface area, no switching

---

## Solution (63 tools across 8 categories)

| Category | # Tools | Capability |
|----------|---------|------------|
| **Form Tools** | 9 | Add/remove/reorder fields, tabs, buttons, separators on entity forms |
| **View & List Tools** | 7 | Configure columns, FetchXML filters, sort order, allowed fields |
| **Workflow & Business Logic** | 8 | Create, validate, explain, and deploy event-driven workflows on forms and views |
| **Data Sync & Filtering** | 6 | Manage FetchXML offline sync rules; read and analyze sync logs |
| **Home Screen & Navigation** | 5 | Add/remove/reorder groups and menu items on app home screen |
| **Configuration & Project** | 15+ | Read entity configs, themes, enabled entities, full project settings |
| **File & Structure Tools** | 10 | Read/write offline HTML files; parse dashboards, maps, calendars, hubs |
| **Initialization & Utilities** | 4+1 | Tool setup per session + JSBridge doc search (public, no auth required) |

**Authentication**: Token-based (`https://agent-dev.resco.net/mcp?token={TOKEN}`), scoped to Dataverse project role.

**Delivery**: MCP server for Claude, Copilot Studio, other MCP-compatible tools. Published to Copilot Studio marketplace.

**NOT in scope**: Multi-org switching | Analytics dashboard | Mobile live preview | Automated code review pipeline

---

## Unfair Advantage

**Strengths**:
- MCP ecosystem mature: 97M+ monthly SDK downloads, 5,800+ servers, enterprise-deployed. Production-ready.
- Copilot Studio marketplace: native MCP support, real distribution channel.
- 63-tool full coverage: not just read/search — AI can actually build and configure Resco apps end-to-end.
- Low cost, high strategic value: cheapest way to accelerate Resco adoption + build Vibe Studio foundation.
- Synergy: MCP provides the AI context layer Vibe Studio needs for both code generation and app configuration.

**Moat**: First-mover only. No tech moat — easily replicable. Speed is the advantage. Even if commoditized, wins if it accelerates Resco adoption and builds Vibe Studio infrastructure.

---

## Channels

**Primary**: Copilot Studio marketplace (organic discovery)

**Early adopters**: 16 Resco partners → 5 internal + 10 partner consultants

**Launch**: Week 1-2 beta → Week 3 marketplace launch → Week 4+ community + webinars

---

## Economics

**Model**: Free tool → more consultants build Resco apps → more projects → more licenses (€10/user/month)

**Per-project**: 20 users × €10/month × 24 months = €4,800

| | Amount |
|---|---|
| Build | €22,500 (1.5 FTE × 3 months) |
| Annual maintenance | €15,000 |
| **Year 1 total** | **€37,500** |
| Break-even Year 1 | 8 projects (156 users) |
| Break-even Year 2+ | 3 projects/year |
| Year 1 forecast | 4-5 projects = €19-24K = **-€13-18K net** |

Profitable Year 2-3 as adoption scales to 11+ projects/year.

---

## Key Metrics

**North Star**: Monthly active consultants using MCP.

| Target | 6 months | 12 months |
|--------|----------|-----------|
| Active users | 20 | 50+ |
| Tool uses | 500+ | — |
| Projects with MCP | — | 8+ |
| End-users on MCP-built UIs | — | 156+ |

---

## Critical Risks

| # | Risk | Severity | Mitigation |
|---|------|----------|------------|
| 1 | **Adoption**: Consultants don't use it | HIGHEST | Beta: need 10/15 regular usage |
| 2 | **Competition**: MS/Resco builds native solution | VERY HIGH | Speed (1-week launch), partnership pivot |
| 3 | **No moat**: Easily replicable | HIGH | None beyond speed |
| 4 | **Value**: Time savings < 5x | MEDIUM | Measure in beta |
| 5 | **Distribution**: Copilot Studio approval delayed | MEDIUM | Claude/other MCP tools as backup |

**Unvalidated**: 10x speed claim | 15K market size | viral coefficient | MS/Resco timeline | consultant tool authority | retention

---

## Next Steps

**THIS WEEK: Beta with 15 consultants** (5 internal + 10 partners)

**Measure**: Usage rate, frequency, time savings, code accuracy, recommendation intent.

| Result | Action |
|--------|--------|
| 10+ regular users | Launch to Copilot Studio marketplace Week 3 |
| 5-9 users | Identify friction, iterate, retest |
| < 5 users | Stop or major pivot |

**Timeline**: Week 1-2 beta → Week 2 go/no-go → Week 3 launch (if validated) → Month 3: 20 users → Month 6: 8+ projects

---

**If MS/Resco announces native MCP**: Pivot to partnership (contribute, don't compete).

**Bottom line**: €37.5K bet. Speed play + Vibe Studio foundation. Even if commoditized, wins by accelerating Resco adoption. Validate adoption THIS WEEK, then decide.

---

*Created: 2026-01-21 | Updated: 2026-03-09 (v4.1 — expanded to 63-tool full toolset) | Next Review: 2026-04-01 | Owner: RESCO Product Team*
