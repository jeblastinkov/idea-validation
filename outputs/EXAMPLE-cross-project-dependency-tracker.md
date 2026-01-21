# Lean Canvas: Cross-Project Dependency Tracker

**Date**: 2026-01-21
**Version**: 1.0
**Status**: Initial Validation

---

## 🎯 Problem

### Top 3 Problems
1. Dev teams lose 5-10 hours/week tracking dependencies manually across projects
2. Delays cascade when cross-project blockers aren't visible until standups
3. No single source of truth - dependencies tracked in Slack, Jira, spreadsheets, tribal knowledge

### Existing Alternatives
- Manual tracking in spreadsheets
- Jira linked issues (doesn't work cross-instance)
- Weekly sync meetings
- Slack threads that get lost

---

## 👥 Customer Segments

### Primary Segment
Engineering Managers at B2B SaaS companies with 50-200 engineers, running multiple concurrent projects with interdependencies

### Early Adopters
EMs who currently use spreadsheets or have tried Jira add-ons but found them inadequate. Companies using monorepo or microservices with shared dependencies.

### Reachability
- LinkedIn (Engineering Manager groups)
- Engineering Manager Slack communities
- Product Hunt launch
- Content marketing (blogs on managing dependencies)

---

## 💎 Unique Value Proposition

### Single, Clear Message
We help engineering managers eliminate dependency tracking overhead by automatically detecting and visualizing cross-project blockers in real-time.

### High-Level Concept
"Dependency tracking that updates itself - like Google Maps for your engineering roadmap"

---

## ✨ Solution

### Top 3 MVP Features
1. **Auto-detection**: Connect to GitHub/GitLab/Jira, automatically identify dependencies from PRs, commits, and tickets
2. **Visual dependency graph**: Real-time visualization of all cross-project dependencies and their status
3. **Automated alerts**: Slack/email notifications when a blocker arises or dependency status changes

### Delivery Channel
Web app (SaaS), with Slack integration for notifications

### NOT in MVP
- Mobile app
- Advanced analytics/reporting
- Team velocity tracking
- Integration with planning tools beyond Jira/GitHub
- Multi-company collaboration
- AI-powered dependency prediction

---

## 🔑 Unfair Advantage

**Network effects from integration**: The more teams use it, the more accurate automatic detection becomes. Our founding team's 15 years combined experience at Google/Meta gives us unique insight into dependency management at scale.

---

## 📊 Channels

### Customer Acquisition
1. **Content marketing**: "How to manage dependencies" blog series, Engineering Manager newsletter
2. **Product Hunt launch**: Target engineering tools audience
3. **LinkedIn outreach**: Direct messages to EMs at target companies
4. **Community presence**: Engineering Manager Slack groups, Reddit r/ExperiencedDevs
5. **Partnerships**: Integration partners (Jira, GitHub, Linear)

### Distribution Strategy
Freemium model: Free for single team, paid for cross-team visibility
Viral loop: When team A depends on team B, invite team B to join

---

## 💰 Revenue Streams

### Revenue Model
Monthly subscription (SaaS), priced per engineering manager

### Pricing
- **Free**: Single team (up to 10 people)
- **Team**: $49/month per manager (2-5 teams)
- **Enterprise**: $99/month per manager (6+ teams) + priority support

### Unit Economics
- LTV: $1,188 (assuming 2-year retention at $49/month)
- Gross margin: 85% (typical SaaS)
- Target LTV:CAC ratio: 5:1

---

## 💸 Cost Structure

### Top Cost Drivers
1. **Infrastructure**: AWS/GCP hosting, database ($500-2K/month scaling with usage)
2. **Engineering**: 2 full-time engineers ($300K/year total comp)
3. **Customer acquisition**: Content, ads, tools ($2-5K/month)

### Customer Acquisition Cost
**Estimated CAC**: $200-300 per customer
- Content marketing: $50-100 (organic)
- Paid ads: $300-500 (if needed)
- Target: <$250 average through content + product-led growth

---

## 📈 Key Metrics

### North Star Metric
**Active cross-team dependencies tracked** (shows product is being used for core value prop)

### Supporting Metrics
- Weekly active teams
- Dependencies detected automatically (vs manually added)
- Blocker notification open rate
- Customer retention (month-over-month)

### Validation Criteria
**Success**:
- 50 teams actively using within 6 months
- 70%+ of dependencies auto-detected (not manual)
- 80%+ month-2 retention

**Failure signals**:
- <20 teams after 3 months
- Most dependencies added manually (auto-detection doesn't work)
- <50% month-2 retention (not valuable enough)

---

## 🚨 Critical Assumptions & Risks

### Riskiest Assumption
**Engineering managers will pay $49-99/month for dependency tracking**

Current behavior: Most use free tools (spreadsheets, Slack, Jira)
Assumption: Enough pain to justify paid tool

### Top 3 Risks
1. **Market Risk**: EMs don't see dependency tracking as valuable enough to pay for
2. **Technical Risk**: Auto-detection accuracy is <70%, requiring too much manual work
3. **Competition Risk**: Jira or Linear adds this feature, eliminates our wedge

### Validation Approach
1. **Week 1-2**: Interview 15 engineering managers
   - How do they track dependencies today?
   - How much time does it cost?
   - Would they pay? How much?

2. **Week 3-4**: Build clickable prototype
   - Show to 10 EMs from interviews
   - Can they understand it?
   - Does it solve their problem?

3. **Week 5-6**: Smoke test pricing
   - Landing page with "Sign up for beta - $49/month"
   - Run $500 in LinkedIn ads
   - Target: 5% click → signup conversion (25 signups from 500 clicks)

4. **Week 7-8**: Concierge MVP
   - Manually track dependencies for 3 teams
   - Deliver daily updates via Slack
   - Test if they find value before building tech

---

## 🎬 Next Steps

### Immediate Action
**Interview 15 engineering managers this week**

Questions:
1. "Tell me about the last time a cross-project dependency caused a delay"
2. "How do you track dependencies today?"
3. "How much time per week does dependency management take?"
4. "What would you pay for a tool that eliminated this overhead?"

### Validation Experiments
1. **Problem validation** (Week 1-2): 15 customer interviews
2. **Solution validation** (Week 3-4): Clickable prototype test
3. **Pricing validation** (Week 5-6): Landing page smoke test
4. **Value validation** (Week 7-8): Concierge MVP with 3 teams

### Timeline
- **Week 8**: Decide build/pivot/stop based on validation results
- **Week 9-12**: Build MVP if validated (only core 3 features)
- **Week 13+**: Beta launch to early adopters from validation

---

## 📝 Notes & Assumptions

### Known Unknowns (TBD)
- Exact pricing point ($49 vs $79 vs $99) - needs testing
- Sales cycle length for B2B SaaS tool
- Integration complexity with various Git/PM tools
- Churn rate (assuming 2-year retention but unvalidated)

### Key Assumptions
- Engineering managers have budget authority for tools <$100/month
- Auto-detection is technically feasible with 70%+ accuracy
- Teams will adopt if EM mandates (not individual contributor buy-in needed)
- 50-200 person companies have 5-10 concurrent projects with dependencies
- Market size: 50K companies × 5 EMs avg = 250K potential users

### Open Questions
- Do we sell to individual EMs or require company-wide adoption?
- Should we offer annual pricing discount?
- Is there a PLG motion (bottom-up adoption by teams)?
- Could this expand to other dependency types (marketing, product, etc.)?

---

## 🔗 Resources

- Customer interview notes: /research/interviews/
- Competitive analysis: Jira, Asana, Monday.com, Linear
- Market sizing: 50K B2B SaaS companies (Source: TBD - needs research)

---

**⚠️ Remember**: This canvas represents assumptions as of 2026-01-21. Every item marked "TBD" or "Estimated" MUST be validated through customer conversations and experiments. The goal is not to perfect this document but to identify and test the riskiest assumptions (pricing, auto-detection accuracy, willingness to pay) before investing in building the product.

**🎯 Focus**: Test pricing and problem severity first through 15 customer interviews. If 10+ of 15 say they'd pay $49+/month, proceed to prototype. If fewer than 5 would pay, pivot or stop.

**💡 Success Criteria**: By end of Week 8, have clear evidence that:
1. Problem is severe (costing 5+ hours/week)
2. EMs will pay $49+ per month
3. Auto-detection is technically feasible
4. Early adopters identified and ready to beta test

**If any of these is invalidated, stop and pivot before building.**
