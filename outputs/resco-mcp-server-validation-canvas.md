# Lean Canvas: Resco MCP Server for AI-Assisted Development

**Date**: 2026-01-21
**Company**: RESCO
**Version**: 1.0
**Status**: Pre-Launch Validation (Launch: 1 week, Announce: 2 weeks)

---

## 🎯 Problem

### Top 3 Problems
1. AI coding assistants (Claude, Copilot, ChatGPT) hallucinate when generating Resco code due to lack of JSBridge documentation context
2. Consultants waste significant time manually searching Resco Wikipedia for documentation and troubleshooting
3. AI tools cannot access client's Dataverse schema, forcing manual entity/field lookups and increasing errors

### Existing Alternatives
- Manual Resco Wikipedia searches (time-consuming, requires deep knowledge)
- ChatGPT with manual doc uploads (incomplete, still hallucinates)
- Hiring developers to build custom HTML with Resco JSBridge logic (expensive, slow)
- Switching to Microsoft Power Platform (abandoning Resco's offline-first advantages)

### Current Workaround Impact
Significant time waste, errors in implementation, steep learning curve, consultant frustration

---

## 👥 Customer Segments

### Primary Segment
**Senior functional consultants** at Microsoft Dynamics 365 implementation partners (100-250 employees) who build Resco mobile apps monthly per project

### Secondary Segment
In-house enterprise teams maintaining business applications on Microsoft ecosystem

### Market Size
- ~15,000 functional consultants globally who work with Resco
- 16 active Resco partners (immediate distribution channel)
- Western Europe and US primarily
- Calculation: 3,000 MS implementation partners × 175 avg employees × 30% consultants × 10% Resco users

### Reachability
1. Resco partner network (16 active partners)
2. Microsoft Copilot Studio marketplace
3. Microsoft Dynamics 365 LinkedIn groups and communities
4. Dynamics 365 conferences and webinars

---

## 💎 Unique Value Proposition

### Single, Clear Message
**"We help functional consultants build Resco apps 10x faster by giving AI assistants direct access to Resco docs and their Dataverse schema—eliminating hallucinations and manual lookups."**

### High-Level Concept
"Like GitHub Copilot, but it actually knows Resco JSBridge and your specific Dataverse structure"

### Why Different from Alternatives
- **vs Manual ChatGPT**: Direct Dataverse connection + full Resco docs (no hallucination)
- **vs vibe.powerapps.com**: Only solution for Resco ecosystem (not Power Apps)
- **vs Manual search**: Automatic context in AI workflow (no context switching)
- **vs Hiring developers**: Enables consultants to build themselves (faster, cheaper)

---

## ✨ Solution

### Top 3 MVP Features (Launch: 1 week)
1. **Resco JSBridge documentation search**: AI-accessible Resco Wikipedia content, eliminating hallucinations
2. **Dataverse schema access**: List entities/tables/fields from client's Dynamics organization for accurate code generation
3. **Sync log analysis**: Troubleshoot Resco mobile app synchronization issues with AI assistance

### Delivery Mechanism
Model Context Protocol (MCP) server compatible with:
- Claude Desktop / Claude Code
- Microsoft Copilot Studio
- Other MCP-compatible AI tools

### Integration
Published to Microsoft Copilot Studio marketplace for one-click installation by consultants

### NOT in MVP (Future)
- Workflow builder tool (#4) - helps build JavaScript business logic
- Code generation templates
- Multi-organization management
- Advanced analytics on usage patterns
- Mobile app preview/testing
- Automated code review

---

## 🔑 Unfair Advantage

**First-mover in Resco ecosystem**: Only MCP server for Resco development, leveraging Resco's unique advantages:
- Offline-first mobile architecture (vs Power Platform online-first)
- Platform-agnostic (Dataverse, Salesforce, ServiceNow backends)
- Native mobile performance
- Enterprise-grade customization

**Distribution advantage**: Direct access to Microsoft Copilot Studio marketplace + established Resco partner network

**Speed to market**: 1 week to launch, establishing category before Microsoft/Resco builds native solution

---

## 📊 Channels

### Customer Acquisition (Free Product)
1. **Resco partner network**: Beta with 16 active partners (80 potential early users)
2. **Microsoft Copilot Studio marketplace**: Primary distribution (organic discovery)
3. **MS Dynamics communities**: LinkedIn groups, forums, Reddit r/Dynamics365
4. **Resco documentation**: Integration into Resco Wikipedia/docs
5. **Partner enablement**: Webinars, demos, hands-on workshops
6. **Conferences**: Dynamics 365 and Resco events (presentations/booth demos)

### Distribution Strategy
1. Week 1-2: Beta test with 5 internal + 10 partner consultants (15 total)
2. Week 3: Launch on Copilot Studio marketplace
3. Week 4+: Community engagement, partner webinars, content marketing

### Viral Loop
Consultants share AI conversations with colleagues → organic spread within partner firms

---

## 💰 Revenue Streams

### Revenue Model
**Indirect revenue growth tool** (MCP server is free)

**Business Logic**:
- Free MCP server → Lowers barrier to Resco development
- More consultants can build Resco apps → More projects delivered
- More projects → More Resco mobile app licenses sold to end customers
- Partners sell Resco to end customers at **€10/user/month**

### Unit Economics (Per Project)
- Average project: 20 mobile end-users
- Resco license revenue: 20 users × €10/month × 24 months average = **€4,800 per project**
- Consultant builds faster → Can deliver more projects → More licenses sold

### Economics Analysis

**Investment**:
- Build cost: 1.5 FTE × 3 months = €22,500
- Annual maintenance: €15,000/year
- **Year 1 total**: €37,500

**Break-Even** (assuming 24-month customer retention):
- Revenue per end-user: €10/month × 24 = €240 lifetime value
- Year 1 break-even: €37,500 / €240 = **156 users = ~8 projects**
- Year 2+ break-even: €15,000 / €240 = **63 users = ~3 projects/year**

**Estimate**: 4-5 new projects in Year 1 (conservative)
- Year 1: 80-100 users = €19,200-24,000 revenue
- **Net Year 1**: -€13,500 to -€18,300 (acceptable investment)
- **Mid-term profitability** (Year 2-3): Expected positive ROI as adoption scales

---

## 💸 Cost Structure

### Development Costs
- **Build (one-time)**: 1.5 FTE × 3 months = €22,500 (avg €60K/year developer cost)
- **Maintenance (ongoing)**: €15,000/year

### Infrastructure Costs
- Hosting MCP server: Minimal (likely <€500/year)
- Microsoft Copilot Studio listing: Free (Microsoft marketplace)
- Resco API usage: Internal (no external cost)

### Marketing/Distribution Costs
- Partner webinars and training: Internal resources
- Documentation and tutorials: Included in maintenance FTE
- Conference presence: Existing Resco marketing budget

### Total Year 1 Investment
**€37,500** (€22,500 build + €15,000 maintenance)

---

## 📈 Key Metrics

### North Star Metric
**Active users**: Unique consultants actively using MCP server monthly

### Success Criteria
- **6 months**: 20 active users (from 16 partners)
- **12 months**: 50+ active users (expanded to broader market)

### Supporting Metrics
1. **MCP connections/tool uses**: Total API calls (engagement depth)
   - Target: 500+ connections in 6 months (25 uses per active user)

2. **Tools usage breakdown**:
   - JSBridge doc searches
   - Dataverse schema queries
   - Sync log analyses

3. **Time reduction**: Measured decrease in Resco HTML development time
   - Target: 10x faster (from consultant feedback)

4. **Projects built using MCP**: Number of Resco projects delivered with MCP assistance
   - Target: 8+ projects in Year 1

5. **Business impact**: Mobile end-users on MCP-built custom UIs
   - Target: 156+ end-users in Year 1 (break-even)

### Tracking Method
- MCP server logs (anonymous usage analytics)
- Partner surveys (quarterly feedback)
- Consultant interviews (qualitative validation)
- Resco license sales correlation analysis

---

## 🚨 Critical Assumptions & Risks

### Riskiest Assumption
**Consultants will actually adopt and use the MCP server in their daily workflow**

**Why risky**:
- Requires behavior change (integrating AI into workflow)
- Consultants may not trust AI-generated code
- Learning curve for MCP setup and usage
- Competing priorities and time constraints

### Top 5 Risks

#### 1. Adoption Risk (HIGHEST)
**Risk**: Consultants don't use MCP despite availability
**Impact**: Zero ROI, wasted €37,500 investment
**Mitigation**: Pre-launch validation with 15 consultants (threshold: 10/15 regular usage)

#### 2. Competition Risk (VERY HIGH)
**Risk**: Microsoft or Resco builds native MCP server before/shortly after launch
**Likelihood**: Very high (acknowledged by stakeholders)
**Impact**: Competitive advantage eliminated, first-mover window closes
**Mitigation**: Speed to market (1 week launch), establish user base quickly, potential partnership discussions

#### 3. Technical Risk (MEDIUM)
**Risk**: MCP accuracy <70%, requires too much manual correction
**Impact**: Tool not valuable, consultants abandon
**Validation**: Test with 15 consultants, measure code accuracy and correction frequency

#### 4. Distribution Risk (MEDIUM)
**Risk**: Microsoft Copilot Studio approval delayed or rejected
**Impact**: Limited distribution reach, dependent on manual sharing
**Mitigation**: Direct integration with Claude/other MCP tools as backup channel

#### 5. Value Risk (MEDIUM)
**Risk**: Time savings <10x, not compelling enough to change behavior
**Impact**: Low adoption, limited viral spread
**Validation**: Measure actual time savings in beta testing phase

### Known Unknowns (TBD - Requires Validation)
- Actual time reduction in real-world consultant workflows (assumed 10x, unvalidated)
- Consultant willingness to integrate AI into delivery process
- Code accuracy rate from MCP-assisted development
- Viral coefficient (do consultants recommend to peers?)
- Microsoft/Resco timeline for native solution (if any)
- Retention rate beyond initial trial period
- Optimal onboarding process for consultants
- Support burden for troubleshooting MCP issues

### Assumptions to Mark
- 15K addressable market (based on estimation, not validated data)
- 20 users/project average (assumed, varies by project type)
- 24-month customer retention (industry average, not Resco-specific)
- 4-5 new projects in Year 1 (conservative estimate, unvalidated)
- 10x faster development claim (marketing claim, needs measurement)
- Consultants have authority to adopt new tools (may require firm approval)

---

## 🎬 Next Steps

### Immediate Validation (Next 2 Weeks)

#### Week 1: Beta Testing
**Action**: Test with 15 consultants (5 internal Resco + 10 from partner firms)

**Validation questions**:
1. Do they actually use it in real project work?
2. Does it reduce development time? By how much?
3. Is code accuracy acceptable?
4. What friction points prevent regular usage?
5. Would they recommend to colleagues?

**Success threshold**: 10 out of 15 use it regularly and report significant value

**Failure signal**: <5 regular users, or feedback that manual methods are faster

#### Week 2: Launch & Announce
- Publish to Microsoft Copilot Studio marketplace
- Announce to partner network
- Create documentation and tutorial videos
- Monitor early adoption metrics

### Validation Experiments

#### Experiment 1: Adoption Test (Weeks 1-2)
**Hypothesis**: 10/15 consultants will use MCP regularly after hands-on demo
**Method**: Demo + 2-week trial with real projects
**Success**: ≥10/15 active users
**Failure**: <5/15 active users → Pivot or stop

#### Experiment 2: Value Validation (Weeks 3-4)
**Hypothesis**: MCP reduces Resco HTML development time by ≥5x
**Method**: Compare time to build identical feature with/without MCP
**Success**: ≥5x faster (even if not 10x)
**Failure**: <2x faster → Insufficient value prop

#### Experiment 3: Viral Spread (Months 2-3)
**Hypothesis**: Consultants recommend MCP to colleagues (viral coefficient >1)
**Method**: Track referral sources of new users
**Success**: >50% of new users from peer recommendations
**Failure**: <20% from recommendations → Need active marketing

#### Experiment 4: Business Impact (Months 4-6)
**Hypothesis**: MCP drives ≥8 new projects in Year 1
**Method**: Survey partners on projects influenced by MCP availability
**Success**: ≥8 projects attributable to MCP
**Failure**: <3 projects → ROI insufficient

### Decision Gates

**Gate 1 (Week 2)**: After beta testing
- ✅ Proceed if 10/15 regular users
- ❌ Pivot if 5-9 users (identify friction, iterate)
- ❌ Stop if <5 users (insufficient adoption)

**Gate 2 (Month 3)**: After initial launch
- ✅ Scale if 20+ active users, positive feedback
- ❌ Reassess if <10 active users
- ❌ Sunset if Microsoft/Resco announces native solution

**Gate 3 (Month 6)**: Mid-year review
- ✅ Continue if trending toward 8+ projects
- ❌ Reduce investment if <4 projects

---

## 📝 Key Insights & Concerns

### Strengths
✅ **Clear problem**: AI hallucination is real pain point for consultants
✅ **First-mover**: No direct competition in Resco MCP space
✅ **Low cost**: €37,500 Year 1 investment is manageable
✅ **Fast launch**: 1 week to MVP, rapid validation cycle
✅ **Distribution**: Copilot Studio marketplace + partner network
✅ **Aligned incentives**: Free tool drives paid licenses

### Concerns
⚠️ **Adoption uncertainty**: Will consultants actually change behavior?
⚠️ **Competition timeline**: Microsoft/Resco may build native solution imminently
⚠️ **No moat**: Easily replicable by larger players
⚠️ **ROI timeline**: Year 1 likely negative, depends on Year 2-3 scaling
⚠️ **Small initial market**: 16 partners = max 80 early users
⚠️ **Unvalidated claims**: 10x speed improvement is assumption, not fact

### Open Questions
❓ What happens if Microsoft/Resco announces native MCP in Week 3?
❓ Can you partner with Microsoft/Resco instead of competing?
❓ Is there a defensible feature beyond "first"?
❓ What if consultants use it but don't convert to projects?
❓ How long until competitors emerge (even if not Microsoft)?

---

## 🎯 Critical First Action

**THIS WEEK: Validate adoption with 15 consultants**

**Setup**:
1. Recruit 5 internal Resco consultants + 10 from partners
2. Provide MCP server setup instructions
3. Assign real project work (build Resco offline HTML for actual client need)
4. Observe usage for 1 week

**Measure**:
- How many actually use it? (target: 10/15)
- How often? (daily/weekly/never)
- What do they build?
- What problems do they encounter?
- Would they pay for it if it weren't free? (willingness to pay = value signal)

**Decision**:
- ✅ **10+ regular users**: Launch to marketplace, proceed
- ⚠️ **5-9 users**: Identify barriers, iterate, retest
- ❌ **<5 users**: Stop or major pivot

**Why this matters**: If consultants won't use it when it's free and you're actively supporting them, they definitely won't use it at scale. Test adoption BEFORE investing in broader distribution.

---

## 🔗 Resources & References

### Competitive Intelligence
- **vibe.powerapps.com**: AI coding tool for Microsoft Power Apps (monitor for Resco expansion)
- **Salesforce**: Building AI-assisted development tools (market trend validation)
- **Microsoft Copilot Studio**: Primary distribution channel

### Market Data
- Microsoft Partner Network: 500K total partners across all products
- Dynamics 365 implementation partners: Estimated 3,000 globally (unvalidated)
- Resco active partners: 16 (confirmed)

### Technical Requirements
- MCP server compatibility with Claude, Copilot Studio, other AI tools
- Secure Dataverse API connection
- Resco Wikipedia/documentation API access
- Sync log parsing capabilities

### Success Examples (Similar Models)
- GitHub Copilot: Free for students/OSS → Drives GitHub adoption
- Stripe developer tools: Free APIs/docs → Drives payment processing revenue
- Twilio documentation: Extensive free resources → Drives usage-based revenue

---

## ⚠️ Final Reality Check

**This is a speed play, not a moat play.**

Your competitive advantage is **launching first and fast** (1 week) before Microsoft/Resco builds native solution. The MCP server itself is easily replicable—there's no defensible technology or network effect.

**Success depends on**:
1. ✅ Consultants actually adopt (validate with 10/15 in beta)
2. ✅ Fast viral spread within partner network (20 users in 6 months)
3. ✅ Converting usage into Resco projects (8+ in Year 1)
4. ⚠️ Microsoft/Resco don't launch competing solution in next 6-12 months

**If Microsoft/Resco announce native MCP**: Consider pivoting to partnership model (contribute your MCP to become official solution) rather than competing.

**Risk-adjusted recommendation**:
- **Proceed** with 1-week launch (low cost, fast validation)
- **Test aggressively** with 15 consultants this week
- **Decide** based on real usage data, not assumptions
- **Move fast** to establish user base before competition emerges
- **Stay flexible** for partnership pivot if Microsoft/Resco builds native

**Remember**: The goal isn't to build a sustainable standalone product—it's to drive Resco license sales. Even if Microsoft/Resco commoditize the MCP, you win if it accelerates Resco adoption in the meantime.

---

**Created**: 2026-01-21
**Next Review**: 2026-02-04 (after beta testing results)
**Owner**: RESCO Product Team
**Status**: Ready for beta validation
