# Resco Studio: ROI Calculator

**Date**: 2026-05-19 | **Version**: 1.0 | **Owner**: Resco Product Team
**Purpose**: Quantify return on investment for Resco Studio adoption at a single enterprise customer account.

> All inputs are adjustable. Defaults are based on: German IT Manager average salary (Glassdoor/PayScale 2025: €44–49/hour gross; conservative internal cost used), validated time savings from product discovery, and Microsoft Power Pages authenticated user pricing (€1.85/user/month annual plan).

---

## Default Assumptions

| Input | Default | Source / Rationale |
|---|---|---|
| IT Manager seats | 1 | Primary persona; 1–4 per account |
| Field Service Manager seats | 2 | Secondary persona; typically more per account than IT Managers |
| IT Manager hourly cost | €50 | Conservative internal cost; German avg gross €44–49/hr (PayScale/Glassdoor 2025) + employer contributions |
| Field Service Manager hourly cost | €40 | Lower than IT Manager; operations/field role |
| IT Manager hours saved / day | 1.5 hrs | Midpoint of 1–2 hrs validated in discovery (Woodford + ChatGPT workflow replaced) |
| Field Service Manager time saved / day | 0.5 hrs | 30 min/day validated — form change requests no longer routed through IT |
| Working days / year | 220 | Standard European working year |
| Resco Studio seat price | €100 / user / month | Published pricing |
| AI credits / month (per account) | €50 | Conservative estimate; TBD from real usage — adjust upward for heavy users |
| External user fee (Resco) | €1.00 / user / month | Target pricing; below Microsoft Power Pages authenticated rate |
| Microsoft Power Pages cost | €1.85 / user / month | Annual plan, authenticated users (Microsoft pricing 2025) |
| External users — Year 1 | 300 | Conservative: hundreds |
| External users — Year 2 | 2,000 | Thousands |
| External users — Year 3 | 15,000 | Tens of thousands |

---

## Year 1 ROI — Base Scenario

### Studio Cost (Annual)

| Item | Calculation | Annual Cost |
|---|---|---|
| IT Manager seat(s) | 1 × €100 × 12 | €1,200 |
| Field Service Manager seat(s) | 2 × €100 × 12 | €2,400 |
| AI credits | €50/month × 12 | €600 |
| External user fees | 300 users × €1.00 × 12 | €3,600 |
| **Total Studio Cost — Year 1** | | **€7,800** |

### Value Delivered (Annual)

| Value Source | Calculation | Annual Value |
|---|---|---|
| IT Manager time savings | 1 seat × 1.5 hrs/day × 220 days × €50/hr | €16,500 |
| Field Service Manager time savings | 2 seats × 0.5 hrs/day × 220 days × €40/hr | €8,800 |
| External user savings vs Microsoft | 300 users × (€1.85 − €1.00) × 12 months | €3,060 |
| **Total Value Delivered — Year 1** | | **€28,360** |

### Year 1 Summary

| Metric | Value |
|---|---|
| Total Studio Cost | €7,800 |
| Total Value Delivered | €28,360 |
| **Net Benefit** | **€20,560** |
| **ROI** | **264%** |
| **Payback Period** | **3.3 months** |

---

## 3-Year Projection — Base Scenario

*Assumptions: seat count constant; AI credits grow 20%/year with usage; external users scale per estimates.*

| | Year 1 | Year 2 | Year 3 | 3-Year Total |
|---|---|---|---|---|
| **COSTS** | | | | |
| Seat licenses | €3,600 | €3,600 | €3,600 | €10,800 |
| AI credits | €600 | €720 | €864 | €2,184 |
| External user fees (Resco) | €3,600 | €24,000 | €180,000 | €207,600 |
| **Total Cost** | **€7,800** | **€28,320** | **€184,464** | **€220,584** |
| | | | | |
| **VALUE** | | | | |
| IT Manager time savings | €16,500 | €16,500 | €16,500 | €49,500 |
| FS Manager time savings | €8,800 | €8,800 | €8,800 | €26,400 |
| External user savings vs MS | €3,060 | €20,400 | €153,000 | €176,460 |
| **Total Value** | **€28,360** | **€45,700** | **€178,300** | **€252,360** |
| | | | | |
| **Net Benefit** | **€20,560** | **€17,380** | **−€6,164** | **€31,776** |
| **ROI** | **264%** | **61%** | **−3%** | **14%** |

> **Note on Year 3**: At 15,000 external users, Resco's fee (€180,000/year) approaches the value delivered from Microsoft savings (€153,000). Year 3 net benefit turns slightly negative in the base scenario — this signals that **external user fee pricing must be reviewed before Year 3 scale**. Either reduce the per-user fee at volume (tiered pricing) or the acquisition value of those 15,000 users must factor into the model.

---

## Sensitivity Analysis — Year 1

### Scenario: Low (1 IT Manager, 1 FS Manager, 1 hr/day saved, 100 external users)

| Metric | Value |
|---|---|
| Total Cost | €4,800 |
| Total Value | €15,700 |
| Net Benefit | €10,900 |
| ROI | **227%** |
| Payback | 3.7 months |

### Scenario: Base (1 IT Manager, 2 FS Managers, 1.5 hrs/day, 300 external users)

| Metric | Value |
|---|---|
| Total Cost | €7,800 |
| Total Value | €28,360 |
| Net Benefit | €20,560 |
| ROI | **264%** |
| Payback | 3.3 months |

### Scenario: High (2 IT Managers, 3 FS Managers, 2 hrs/day, 1,000 external users)

| Metric | Value |
|---|---|
| Total Cost | €18,600 |
| Total Value | €64,540 |
| Net Benefit | €45,940 |
| ROI | **247%** |
| Payback | 3.5 months |

**Key finding**: ROI is consistently 227–264% in Year 1 across all scenarios. Payback period is under 4 months in every case. The investment thesis for Resco Studio is strong at account level — the payback is fast enough that even skeptical buyers can justify a trial.

---

## External Data Collection — Standalone ROI

*For customers whose primary use case is replacing Microsoft Power Pages for external users.*

| External Users / Month | Microsoft Cost (annual) | Resco Cost (annual) | Annual Saving |
|---|---|---|---|
| 100 | €2,220 | €1,200 | €1,020 |
| 500 | €11,100 | €6,000 | €5,100 |
| 1,000 | €22,200 | €12,000 | €10,200 |
| 5,000 | €111,000 | €60,000 | €51,000 |
| 10,000 | €222,000 | €120,000 | €102,000 |
| 50,000 | €1,110,000 | €600,000 | €510,000 |

> Microsoft cost = €1.85/authenticated user/month × 12. Resco cost = €1.00/user/month × 12.
> At scale, the saving becomes the headline — not "Resco is cheaper" but "Resco saves you €510K/year vs Microsoft at 50K external users."

**Pricing sensitivity**: If Resco prices at €0.50/user/month (half the default), annual saving at 50K users = **€810K vs Microsoft**. The lower the fee, the stronger the acquisition argument — find the floor that still generates meaningful Resco revenue.

---

## Key Takeaways for Sales Conversations

1. **Payback under 4 months** — in every scenario, Studio pays for itself before Q2 of year 1. This eliminates the "it's too expensive" objection.

2. **Time savings alone justify the seat cost** — even ignoring external users and AI credits, IT Manager time savings (€16,500/year) cover the total seat cost (€3,600/year) by 4.6×.

3. **External user scale is where the big numbers live** — at 10,000+ external users, the Microsoft savings comparison becomes the primary ROI driver, dwarfing seat economics.

4. **Tiered external user pricing needed at scale** — the model shows Year 3 economics tighten as external user fees grow. Build a volume discount tier (e.g., €0.50/user/month above 5,000 users) before customers hit that wall.

5. **Field Service Manager ROI is the easiest conversation** — 30 minutes/day saved × 220 days × €40/hour = €8,800/year per 2 FS Manager seats costing €2,400. The math is immediate and requires no technical explanation.

---

## Assumptions to Validate

| Assumption | How to validate |
|---|---|
| 1.5 hrs/day IT Manager time savings | Time-and-motion study with 5 beta customers — track hours in Woodford+ChatGPT vs Studio |
| 30 min/day FS Manager savings | Survey beta users: time from form change request to live, before and after |
| €50 AI credits/month | Instrument first 20 paying accounts; establish P10/P50/P90 consumption range |
| €1.00/external user/month pricing | Customer WTP interviews; benchmark against Power Pages at different volume tiers |
| External user volumes (300 / 2K / 15K) | Qualify in sales discovery: "How many contractors/suppliers submit data to you monthly?" |

---

**Sources**:
- IT Manager salary: [PayScale Germany 2025](https://www.payscale.com/research/DE/Job=Information_Technology_(IT)_Manager/Salary) | [Glassdoor Germany 2025](https://www.glassdoor.com/Salaries/germany-it-manager-salary-SRCH_IL.0,7_IN96_KO8,18.htm)
- Microsoft Power Pages pricing: [Microsoft Power Platform](https://www.microsoft.com/en-us/power-platform/products/power-pages/pricing) | [The Portal Company 2025](https://www.theportalcompany.com/resources/how-to-licence-power-pages/)

*Created: 2026-05-19 | Next review: After first 20 paying accounts establish real usage baseline*
