# Lean Canvas: RESCO AI Vibe Studio

**Date**: 2026-02-06 | **Company**: RESCO | **Version**: 1.0 | **Status**: Initial Validation

---

## 📋 Executive Summary

**Idea**: Web-based AI-powered development studio (vibe.resco.net) that lets business app makers build, preview, and publish Resco Mobile Apps through natural language prompts and live device preview — replacing the manual Woodford + code workflow

**Target**: ~15,000 functional consultants and solution architects at Resco/Microsoft Dynamics partners globally, plus enterprise in-house teams

**Economics**: €200-300K Year 1 investment (3-5 FTE build + infrastructure + AI costs), revenue via Resco license uplift (€10/user/month) + potential Vibe Studio subscription tier — TBD - Requires pricing validation

**Risk**: Business app makers won't adopt AI-first workflow over established Woodford/manual coding habits; Microsoft's vibe.powerapps.com may make Resco-specific tooling irrelevant

**Next Action**: Run a 2-week closed beta with 10-15 existing Resco partners building real UIReplacement apps, measuring time-to-first-app vs. current workflow

---

## 🎯 Problem

### Top 3 Problems
1. **Slow build-test cycle**: Building Resco mobile apps (UIReplacements, form components) requires manual Woodford configuration + coding + sync + device testing — a cycle that takes hours-to-days per iteration with no live preview capability
2. **High skill barrier**: Creating custom Resco mobile apps demands deep knowledge of JSBridge APIs, Woodford metadata, and backend schemas (Dataverse/Salesforce/ServiceNow) — most functional consultants lack this, forcing reliance on scarce developers
3. **No modern developer experience**: Resco app development has no web-based IDE, no AI assistance, no instant preview — falling behind the "vibe coding" trend where competitors offer AI-generated apps in minutes

### Existing Alternatives
- **Woodford** (Resco's config tool): Powerful but complex, no live preview, steep learning curve, requires deep platform expertise
- **Manual JSBridge coding**: Requires developer skills, tedious debug cycle, no AI context for Resco APIs
- **ChatGPT/Copilot with uploaded docs**: Hallucinate Resco APIs, no Dataverse schema access, incomplete context
- **Switch to Power Apps**: Lose Resco's offline-first, multi-backend, and native mobile advantages

---

## 👥 Customer Segments

**Primary**: Senior functional consultants and solution architects at Microsoft Dynamics 365 implementation partners (100-500 employees) who build or customize Resco mobile apps for client projects

**Secondary**: In-house enterprise IT teams maintaining Resco MobileCRM deployments; ISVs building vertical solutions on the Resco platform

**Market size**: ~15,000 Resco-adjacent consultants globally (3,000 MS partners × 175 avg employees × 30% consultants × 10% Resco scope) | 16 active Resco partners (immediate reach, ~80 direct users) | Western Europe and US primarily

**Reachability**: Resco partner network (16 partners, direct relationships) | Resco events/conferences | Microsoft Dynamics LinkedIn groups | Resco documentation site integration | Partner account managers as channel

---

## 💎 Unique Value Proposition

**"We help business app makers build and deploy Resco mobile apps in minutes instead of days, using AI-assisted code generation with live device preview — no deep coding expertise required."**

**High-level concept**: "Like Lovable/Bolt.new, but purpose-built for Resco Mobile Apps — connected to your backend and your mobile project"

**Why different**:
- vs **Woodford**: AI-driven, live preview on device, modern web IDE — not manual metadata configuration
- vs **vibe.powerapps.com**: Native Resco offline-first + multi-backend (Dataverse + Salesforce + ServiceNow) — not locked to Microsoft online-only
- vs **Lovable/Bolt/v0**: Deep Resco ecosystem integration — understands mobile project metadata, JSBridge APIs, backend schemas via MCP server
- vs **Manual AI coding** (ChatGPT/Copilot): Zero hallucination on Resco APIs + direct Dataverse schema access + instant on-device preview

---

## ✨ Solution

### Top 3 MVP Features (Phase 1 — UIReplacement)
1. **Environment + AI code generation**: Web workspace at vibe.resco.net — connect to backend (Dataverse/Salesforce/ServiceNow/RescoCloud), select or create a mobile project, describe the app in natural language → AI (Copilot/Claude + Resco MCP server) generates UIReplacement code with real-time progress messages
2. **Monaco editor with code view**: Generated code displayed in embedded Monaco editor for review, manual editing, and iterative prompting — developer remains in control of the output
3. **QR-based live device preview + publish**: Scan QR code to get the app on a physical device with auto-refresh on code changes (live dev mode); publish button to push current bundle to production while continuing development

### Delivery Channel
Web application at vibe.resco.net (browser-based, no local installation)

### NOT in MVP
- Form Components (visible but disabled in UI)
- AI Assistants / AI Pantheon (visible but disabled)
- Questionnaire builder (visible but disabled)
- List Components (TBD)
- Marketplace for tools/snippets
- Multi-user collaboration
- PDF/export of generated apps

---

## 🔑 Unfair Advantage

**Platform owner advantage**: Only Resco can build a deeply integrated Vibe Studio — proprietary access to Woodford metadata APIs, mobile project structure, offlinehtml deployment pipeline, and sync infrastructure. Third parties cannot replicate this integration depth.

**MCP server synergy**: Resco MCP server (already in development/validation) provides the AI context layer — JSBridge documentation, Dataverse schema access, sync log analysis — that makes AI code generation accurate rather than hallucination-prone.

**Captive distribution**: 16 active partners with direct account manager relationships = built-in beta channel and go-to-market without paid acquisition.

**Reality check**: The platform-owner moat is real but the broader trend favors Microsoft (vibe.powerapps.com). Resco's advantage holds only while offline-first + multi-backend differentiation matters to customers.

---

## 📊 Channels

**Primary**: Resco partner network — direct outreach through account managers, partner webinars, and technical enablement sessions

**Early adopters**: Existing Resco partners already building UIReplacement apps — they know the pain, have active projects, and can validate immediately

**Community/Content**: Resco documentation site (embedded), Microsoft Dynamics LinkedIn groups, Resco annual conference, partner technical forums

**Launch strategy**: Month 1 closed beta (10-15 partners) → Month 2-3 open beta (all partners) → Month 4 public launch at vibe.resco.net → Month 6+ community marketplace

**Viral loop**: Consultant builds app with Vibe Studio → demos to client → client requests more apps → consultant becomes repeat user → recommends to peers at partner firm

---

## 💰 Economics

**Revenue model**: Dual-stream
- **Indirect (primary)**: Free/freemium Vibe Studio drives new Resco Mobile CRM license sales (€10/user/month) — same model as MCP server
- **Direct (future)**: Vibe Studio Pro subscription for advanced features (multiple environments, team collaboration, priority AI, marketplace access) — TBD - Requires pricing validation

**Per-project revenue** (indirect): 20 mobile end-users (avg) × €10/month × 24 months retention = €4,800 per project

**Investment**:
- Build: 3-5 FTE × 6 months = €150-250K (web platform, Monaco integration, QR preview, MCP integration, backend connectors)
- AI/LLM costs: €20-40K/year (API calls for code generation — scales with usage)
- Ongoing maintenance: €80-120K/year (2-3 FTE)
- **Total Year 1**: €250-400K

**Break-even** (on indirect license revenue alone):
- €300K (midpoint) / €4,800 per project = 63 projects needed
- At 5 projects/partner × 16 partners = 80 projects achievable in Year 1-2
- Break-even: ~12-18 months (conservative)

**Forecast**: 30-50 projects Year 1 (conservative) = €144-240K indirect revenue = net -€60-160K (acceptable platform investment)

**Profitability**: Year 2 if adoption scales + direct subscription revenue added

---

## 📈 Key Metrics

**North Star**: Apps deployed to devices via Vibe Studio (measures full value delivery end-to-end)

**Success criteria**:
- 3 months (beta): 15 active users, 30 apps created, time-to-first-app < 1 hour
- 6 months: 50 active users, 150 apps deployed, 20+ projects using Vibe Studio-built apps in production
- 12 months: 100+ active users, 500 apps, measurable uplift in Resco license pipeline

**Supporting metrics**:
- Time-to-first-app: Target < 30 minutes (vs current days-to-weeks) — primary value proof
- AI code generation success rate: > 70% of generated code runs without manual fixes
- Live preview sessions per user per week: > 5 (engagement depth)
- Environments connected: Growth rate of backend connections (stickiness signal)
- Return rate: WAU/MAU > 40% (indicates habit formation)

**Tracking**: Vibe Studio analytics (usage logs) | Partner surveys (quarterly NPS) | Resco license correlation (CRM pipeline data) | Beta user interviews

---

## 🚨 Critical Risks

**Riskiest assumption**: Business app makers will adopt an AI-first workflow for Resco app development instead of sticking with Woodford and manual coding. This requires a significant behavior change — and the primary users (functional consultants) are not developers who naturally gravitate toward IDEs and AI coding tools.

**Top 5 Risks**:

1. **Adoption risk (HIGHEST)**: Functional consultants prefer Woodford's familiar drag-and-configure approach over a code-generating AI tool → Low usage despite investment
   - *Mitigation*: Closed beta with 10-15 partners on real projects; measure time savings and preference; iterate on UX for non-developer persona

2. **Competition risk (HIGH)**: Microsoft launches/expands vibe.powerapps.com with offline and multi-backend capabilities → Resco's differentiation narrows and partners migrate
   - *Mitigation*: Ship fast (first-mover in Resco ecosystem); position as complementary to PowerApps for offline/multi-backend scenarios; monitor Microsoft roadmap quarterly

3. **AI quality risk (HIGH)**: Generated Resco UIReplacement code is unreliable, produces runtime errors, or fails on edge cases → Users lose trust after first attempt
   - *Mitigation*: Invest in MCP server quality (JSBridge doc completeness, schema accuracy); extensive testing with real projects before beta; allow manual code editing as fallback

4. **Scope risk (MEDIUM)**: UIReplacement-only MVP is too narrow — partners need Form Components, AI Assistants, and Questionnaires to see full value → "Nice demo but not useful for my real work"
   - *Mitigation*: Validate with beta users whether UIReplacement alone drives adoption; fast-follow with Form Components in Phase 2; show disabled features to signal roadmap commitment

5. **Technical complexity risk (MEDIUM)**: Multi-backend + live preview + MCP + Monaco + QR device sync = significant integration surface area → Delays, bugs, unstable experience
   - *Mitigation*: Start with single backend (Dataverse) in beta; add Salesforce/ServiceNow post-validation; limit initial scope to proven tech stack

**Key unknowns**:
- Will functional consultants (non-developers) use a code editor-based tool? — TBD - Requires validation
- What's the actual time savings vs. Woodford for real-world projects? — TBD - Requires measurement
- Will AI-generated Resco code quality be good enough? — TBD - Requires testing with MCP server
- Microsoft's timeline for expanding vibe.powerapps.com — TBD - External dependency
- Pricing tolerance for a direct subscription tier — TBD - Requires validation

**Assumptions to validate**:
- 15K addressable market (estimation, not validated)
- Functional consultants will adopt a code-editor workflow (behavior change)
- MCP server provides sufficient context for accurate code generation
- Live preview via QR code is technically reliable across platforms
- 20 users per project average (varies by project type)
- Partners will promote Vibe Studio to their consultants
- AIReplacement-only MVP is sufficient for initial traction
- RescoCloud can serve as a "no backend" option for trial users

---

## 🎬 Next Steps

**THIS MONTH: Closed beta with 10-15 Resco partners building real UIReplacement apps**

**Setup**:
- Recruit: 5 internal Resco + 10 from top partner firms (select partners already building UIReplacements)
- Provide: Working prototype with Dataverse backend support + Monaco editor + QR preview
- Task: Each participant builds one real UIReplacement app for an actual client project
- Duration: 2 weeks active usage

**Measure**:
- Time-to-first-app (target: < 1 hour vs. current days)
- AI code generation accuracy (target: > 70% runs without manual fix)
- Completion rate (how many finish a working app?)
- Would use again? (NPS / preference vs. Woodford)
- Live preview reliability (QR success rate across iOS/Android)

**Decision criteria**:
- ✅ **10+ users complete a working app, > 50% prefer Vibe Studio over Woodford**: Proceed to open beta Month 3
- ⚠️ **5-9 users complete, mixed feedback**: Identify friction points (is it UX? AI quality? scope?), iterate, retest
- ❌ **< 5 users complete or strong Woodford preference**: Reassess — either pivot UX away from code editor or scope down to "AI-assisted Woodford" rather than full Vibe Studio

**Timeline**:
- Month 1: Build MVP prototype (Dataverse + UIReplacement + Monaco + QR preview)
- Month 2: Closed beta (10-15 partners)
- Month 2 end: Go/no-go decision based on beta results
- Month 3-4: Open beta (all partners) + iterate based on feedback
- Month 5-6: Public launch at vibe.resco.net + Phase 2 planning (Form Components)

**Why this matters**: The entire bet rests on whether non-developer business app makers will adopt an AI+code workflow. If they won't use it in a supported beta with real projects, they won't use it at scale. Validate the behavior change BEFORE building out Form Components, AI Assistants, and marketplace.

---

## 📝 Key Assumptions

- ~15,000 addressable Resco-adjacent consultants globally (estimation, not validated)
- Functional consultants will use a code editor + AI workflow (significant behavior change — TBD)
- Resco MCP server provides sufficient context for accurate code generation (depends on MCP maturity)
- Live device preview via QR code is technically reliable (untested at scale)
- UIReplacement-only MVP is sufficient to demonstrate value (may be too narrow)
- 20 mobile end-users per project on average (varies significantly by project type)
- Partners will actively promote Vibe Studio to their consulting teams
- AI/LLM costs remain economically viable at scale (~€20-40K/year estimate)
- Microsoft does not expand vibe.powerapps.com to cover offline + multi-backend (external risk)
- "Try for free without registration" lowers barrier enough for trial adoption

---

## ⚠️ Reality Check

**This is a platform play with a real moat but a real risk.** Unlike the MCP server (low cost, fast launch), Vibe Studio requires significant investment (€250-400K Year 1) and depends on a behavior change from consultants who may prefer what they know. The moat is genuine — only Resco can build this level of integration — but Microsoft's vibe.powerapps.com signals that the "AI app builder" space is being commoditized at the platform level.

**Success depends on**:
1. Non-developer consultants actually adopting an AI+code workflow (the fundamental bet)
2. MCP server delivering accurate enough code generation to build trust on first use
3. Live preview working reliably enough to feel "magical" vs. the current sync-and-test cycle
4. Microsoft not closing the offline/multi-backend gap before Resco establishes Vibe Studio adoption

**If Microsoft expands vibe.powerapps.com to offline + multi-backend**: Pivot Vibe Studio to become the "Resco layer" on top of Power Apps — an embedded experience rather than a standalone platform. The AI assistance + Resco-specific context remains valuable even if the hosting platform changes.

**If adoption fails (consultants reject code editor)**: Consider pivoting to "AI-assisted Woodford" — keep the AI and live preview but wrap it in Woodford's familiar drag-and-configure UX instead of a Monaco editor. The underlying AI value may still hold even if the IDE form factor doesn't.

**Remember**: The goal is making Resco app development 10x faster and accessible to non-developers. If Vibe Studio achieves that, it becomes Resco's primary competitive moat against Power Apps. If it doesn't, the investment is significant. Validate fast, validate cheap.

---

**Created**: 2026-02-06 | **Next Review**: 2026-02-20 (post-beta planning) | **Owner**: RESCO Product Team
