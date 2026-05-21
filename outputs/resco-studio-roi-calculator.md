# Resco Studio: ROI Calculator

**Date**: 2026-05-19 | **Version**: 1.1 | **Owner**: Resco Product Team
**Purpose**: Quantify return on investment for Resco Studio adoption at a single enterprise customer account.

> Defaults based on: German IT Manager average salary (Glassdoor/PayScale 2025: €44–49/hour gross; conservative internal cost used), validated time savings from product discovery, and Microsoft Power Pages authenticated user pricing (€1.85/user/month annual plan, packs of 100).

---

## Default Assumptions

| Input | Default | Source / Rationale |
|---|---|---|
| IT Manager seats | 1 | Primary persona; 1–4 per account |
| Field Service Manager seats | 2 | Secondary persona |
| IT Manager hourly cost | €50 | Conservative internal cost; German avg gross €44–49/hr (PayScale/Glassdoor 2025) + employer contributions |
| Field Service Manager hourly cost | €40 | Operations/field role |
| IT Manager hours saved / day | 1.5 hrs | Midpoint of 1–2 hrs validated in discovery |
| Field Service Manager time saved / day | 0.5 hrs | 30 min/day validated — form changes no longer routed through IT |
| Working days / year | 220 | Standard European working year |
| Resco Studio seat price | €100 / user / month | Published pricing |
| AI credits / month (per account) | €50 | Conservative estimate; TBD from real usage |
| **External user fee (Resco)** | **€3.00 / user / month** | **Confirmed pricing** |
| Microsoft Power Pages — annual plan | €1.85 / user / month | Authenticated users, sold in packs of 100 (Microsoft 2025) |
| Microsoft Power Pages — pay-as-you-go | €3.70 / user / month | No annual commitment (Microsoft 2025) |
| External users — Year 1 | 300 | Conservative: hundreds |
| External users — Year 2 | 2,000 | Thousands |
| External users — Year 3 | 15,000 | Tens of thousands |

---

## ⚠️ Critical Finding: External User Pricing vs Microsoft

At **€3.00/user/month**, Resco is:
- **More expensive** than Microsoft Power Pages annual plan (€1.85/user) for volumes above ~62 users/month
- **Cheaper** than Microsoft Power Pages pay-as-you-go (€3.70/user) at all volumes
- **Cheaper** than Microsoft annual plan below 62 users/month (due to Microsoft's minimum pack of 100 users = €185/month floor)

| Volume | Microsoft Annual | Microsoft PAYG | Resco (€3) | vs MS Annual | vs MS PAYG |
|---|---|---|---|---|---|
| 50 users | €185/mo (pack min) | €185/mo | €150/mo | **Resco saves €35** | **Resco saves €35** |
| 62 users | €185/mo (pack min) | €230/mo | €186/mo | Break-even | **Resco saves €44** |
| 100 users | €185/mo | €370/mo | €300/mo | Resco costs €115 more | **Resco saves €70** |
| 500 users | €925/mo | €1,850/mo | €1,500/mo | Resco costs €575 more | **Resco saves €350** |
| 1,000 users | €1,850/mo | €3,700/mo | €3,000/mo | Resco costs €1,150 more | **Resco saves €700** |
| 5,000 users | €9,250/mo | €18,500/mo | €15,000/mo | Resco costs €5,750 more | **Resco saves €3,500** |

**Bottom line**: At €3.00, Resco is **not competitive vs Microsoft annual plan** above 62 users/month. The external user cost savings story — which was a primary acquisition argument — **does not hold at this price point** against customers with annual Microsoft agreements.

**However, the time savings ROI remains strong** — Studio still pays for itself, just on a longer timeline and primarily through productivity gains, not licensing savings.

---

## Year 1 ROI — Base Scenario (300 external users)

### Studio Cost (Annual)

| Item | Calculation | Annual Cost |
|---|---|---|
| IT Manager seat(s) | 1 × €100 × 12 | €1,200 |
| Field Service Manager seat(s) | 2 × €100 × 12 | €2,400 |
| AI credits | €50/month × 12 | €600 |
| External user fees | 300 users × **€3.00** × 12 | **€10,800** |
| **Total Studio Cost — Year 1** | | **€15,000** |

### Value Delivered (Annual)

| Value Source | Calculation | Annual Value |
|---|---|---|
| IT Manager time savings | 1 seat × 1.5 hrs/day × 220 days × €50/hr | €16,500 |
| Field Service Manager time savings | 2 seats × 0.5 hrs/day × 220 days × €40/hr | €8,800 |
| External user cost vs MS annual | 300 × (€1.85 − **€3.00**) × 12 | **−€4,140** ⚠️ |
| External user cost vs MS PAYG | 300 × (€3.70 − €3.00) × 12 | +€2,520 |
| **Total Value (vs MS annual)** | | **€21,160** |
| **Total Value (vs MS PAYG)** | | **€27,820** |

> The external user line is **negative vs Microsoft annual plan** — Resco costs more per user at this pricing. Value is delivered entirely through time savings. The PAYG comparison is favourable but most enterprise customers are on annual agreements.

### Year 1 Summary

| Metric | vs MS Annual | vs MS PAYG |
|---|---|---|
| Total Studio Cost | €15,000 | €15,000 |
| Total Value Delivered | €21,160 | €27,820 |
| **Net Benefit** | **€6,160** | **€12,820** |
| **ROI** | **41%** | **85%** |
| **Payback Period** | **8.5 months** | **6.5 months** |

*Previous v1.0 calculation (at €1.00/user): 264% ROI, 3.3 month payback. The change to €3.00 reduces Year 1 ROI from 264% to 41% in the base scenario.*

---

## 3-Year Projection — Base Scenario

*Seat count constant; AI credits grow 20%/year; external users scale per estimates.*

| | Year 1 | Year 2 | Year 3 | 3-Year Total |
|---|---|---|---|---|
| **COSTS** | | | | |
| Seat licenses | €3,600 | €3,600 | €3,600 | €10,800 |
| AI credits | €600 | €720 | €864 | €2,184 |
| External user fees (Resco €3) | €10,800 | €72,000 | €540,000 | €622,800 |
| **Total Cost** | **€15,000** | **€76,320** | **€544,464** | **€635,784** |
| | | | | |
| **VALUE** | | | | |
| IT Manager time savings | €16,500 | €16,500 | €16,500 | €49,500 |
| FS Manager time savings | €8,800 | €8,800 | €8,800 | €26,400 |
| Ext. user savings vs MS annual | −€4,140 | −€27,600 | −€207,000 | −€238,740 |
| **Total Value (vs MS annual)** | **€21,160** | **−€2,300** | **−€181,700** | **−€162,840** |
| | | | | |
| **Net Benefit** | **+€6,160** | **−€78,620** | **−€726,164** | **−€798,624** |
| **ROI** | **41%** | **−103%** | **−133%** | **−126%** |

> **Year 2 and Year 3 are deeply negative.** At 2,000 external users (Year 2), the Resco fee (€72,000) already exceeds total value delivered (−€2,300 net). At 15,000 users (Year 3), Resco costs the customer €726K more than it delivers in value. **This pricing model cannot scale with external user growth.**

---

## Sensitivity Analysis — Year 1

### Scenario: Low (1 IT Manager, 1 FS Manager, 1 hr/day saved, 100 external users)

| Metric | Value |
|---|---|
| Total Cost | €6,600 |
| Total Value (vs MS annual) | €14,020 |
| Net Benefit | **+€7,420** |
| ROI | **112%** |
| Payback | 5.6 months |

> At 100 users, Resco (€300/mo) is pricier than MS annual pack minimum (€185/mo), but the volume difference (100 actual users vs paying for 100 either way) makes it manageable. Time savings carry the ROI.

### Scenario: Base (1 IT Manager, 2 FS Managers, 1.5 hrs/day, 300 external users)

| Metric | Value |
|---|---|
| Total Cost | €15,000 |
| Total Value (vs MS annual) | €21,160 |
| Net Benefit | **+€6,160** |
| ROI | **41%** |
| Payback | 8.5 months |

### Scenario: High (2 IT Managers, 3 FS Managers, 2 hrs/day, 1,000 external users)

| Metric | Value |
|---|---|
| Total Cost | €42,600 |
| Total Value (vs MS annual) | €43,400 |
| Net Benefit | **+€800** |
| ROI | **1.9%** ⚠️ |
| Payback | ~11.8 months |

> At 1,000 external users the ROI collapses to near-zero. The time savings value (€57,200) is almost entirely consumed by the excess external user cost vs Microsoft annual (−€13,800). A customer with 1,000+ external users on a Microsoft annual agreement has no financial case for Resco external data collection at €3/user.

---

## External Data Collection — Standalone Feasibility at €3/user

*For customers considering Resco Studio purely for external data collection (no seat licenses).*

| Ext. Users/Month | MS Annual/yr | MS PAYG/yr | Resco €3/yr | vs MS Annual | vs MS PAYG |
|---|---|---|---|---|---|
| 50 | €2,220 | €2,220 | €1,800 | **Save €420** | **Save €420** |
| 62 | €2,220 | €2,759 | €2,232 | Break-even | **Save €527** |
| 100 | €2,220 | €4,440 | €3,600 | **Cost +€1,380** | **Save €840** |
| 500 | €11,100 | €22,200 | €18,000 | **Cost +€6,900** | **Save €4,200** |
| 1,000 | €22,200 | €44,400 | €36,000 | **Cost +€13,800** | **Save €8,400** |
| 5,000 | €111,000 | €222,000 | €180,000 | **Cost +€69,000** | **Save €42,000** |
| 10,000 | €222,000 | €444,000 | €360,000 | **Cost +€138,000** | **Save €84,000** |

**Feasibility verdict at €3.00/user/month**:
- ✅ **Viable vs Microsoft PAYG** at all volumes — Resco saves 19% consistently
- ✅ **Viable vs Microsoft annual** only below ~62 users/month
- ❌ **Not viable vs Microsoft annual** above 62 users — and most enterprise customers are on annual agreements
- ❌ **Not viable at scale** — at Year 2–3 volumes (2K–15K users), the Resco fee becomes the dominant cost and destroys account-level ROI

---

## Pricing Recommendation

**€3.00/user/month is too high for the external data collection value proposition to work as an acquisition driver at scale.** The numbers are honest and the conclusion is clear.

### Option A — Tiered volume pricing (Recommended)

| Monthly external users | Price / user / month | Annual revenue at each tier |
|---|---|---|
| 1 – 500 | €3.00 | Up to €18,000 |
| 501 – 5,000 | €1.50 | €9,000 – €90,000 |
| 5,001 – 20,000 | €0.75 | €45,000 – €180,000 |
| 20,001+ | €0.40 | Negotiate |

- Maintains strong margin at low volumes where Microsoft minimum packs make Resco competitive
- Restores competitive positioning vs Microsoft annual plan at medium/large volumes
- Creates a natural growth path: customers start small, scale with predictable cost

### Option B — Flat lower price (€1.00–€1.50/user/month)

- Undercuts Microsoft annual at all volumes
- Restores the acquisition narrative ("always cheaper than Microsoft")
- Reduces per-unit revenue but significantly expands addressable market
- At €1.50/user: Resco saves customers 19% vs Microsoft annual at any volume

### Option C — Keep €3.00 but reframe the value story

- Stop positioning external data collection as a cost-saving vs Microsoft
- Position on **simplicity and speed**: "no portal setup, no developer, AI-built forms in minutes"
- Quantify the Power Pages portal development cost (typically €10,000–€50,000 professional services) and amortize it — at those numbers, €3/user looks different
- Only works for customers who don't already have a Power Pages deployment

---

## Revised Key Takeaways for Sales Conversations

1. **Lead with time savings, not external user pricing.** At €3/user, the external data collection feature is not cheaper than Microsoft annual. Time savings (IT Manager + FS Manager) still deliver strong ROI — 41–112% in Year 1 — and that is the primary sales argument.

2. **External data collection is a land-and-expand play, not a cost-savings play.** Position it as capability Resco has that Microsoft makes painful — not as "cheaper than Microsoft." The value is simplicity, AI-built forms, and no portal setup — not licensing cost.

3. **Qualify external user volume in discovery.** If a prospect has >500 external users/month on a Microsoft annual agreement, the current €3 pricing makes the external data feature an ROI liability, not an asset. Know this before the demo.

4. **Tiered pricing is necessary before scaling external users.** Volume must trigger a lower per-unit rate or the product destroys customer ROI at Year 2–3 growth. This is not optional — it must be in the roadmap before any customer reaches 1,000+ external users/month.

5. **The seat ROI story is still clean.** IT Manager time savings (€16,500/year) alone cover all seat costs (€3,600/year) by 4.6×. That conversation stands regardless of external user pricing.

---

## Assumptions to Validate

| Assumption | How to validate |
|---|---|
| 1.5 hrs/day IT Manager time savings | Time-and-motion study with 5 beta customers |
| 30 min/day FS Manager savings | Survey beta users: before/after form change cycle time |
| €50 AI credits/month | Instrument first 20 paying accounts; P10/P50/P90 range |
| External user volumes (300 / 2K / 15K) | Qualify in sales discovery: "How many external parties submit data monthly?" |
| Microsoft annual vs PAYG prevalence | Ask in discovery: "Are you on a Power Pages annual plan?" — determines which comparison applies |
| Power Pages portal setup cost | Research professional services market rate; amortize against Resco's zero-setup advantage |

---

**Sources**:
- IT Manager salary: [PayScale Germany 2025](https://www.payscale.com/research/DE/Job=Information_Technology_(IT)_Manager/Salary) | [Glassdoor Germany 2025](https://www.glassdoor.com/Salaries/germany-it-manager-salary-SRCH_IL.0,7_IN96_KO8,18.htm)
- Microsoft Power Pages pricing: [Microsoft Power Platform](https://www.microsoft.com/en-us/power-platform/products/power-pages/pricing) | [The Portal Company 2025](https://www.theportalcompany.com/resources/how-to-licence-power-pages/)

*Created: 2026-05-19 | Updated: 2026-05-19 (v1.1 — corrected external user fee to €3.00) | Next review: After first 20 paying accounts*
