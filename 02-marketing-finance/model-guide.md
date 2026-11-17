# Marketing finance model guide

Open `mmos-marketing-finance.xlsx` in Excel. **Blue numeric inputs** are assumptions; calculated cells are formulas. No Python is needed to use the model.

## Workbook tabs

| Tab | Role |
|---|---|
| `Inputs` | Simulated company revenue, costs, sales assumptions, and pilot inputs |
| `Marketing Budget` | Annual investment by activity and quarterly allocation |
| `Marketing Funnel` | Simulated lead-generation and conversion economics by activity |
| `Pilot ROI` | Incremental *scenario*, not proven attribution |
| `Company P&L` | Full operating P&L with pilot impact, accounting context |
| `Management View` | KPIs and decision points for management |

## The central boundary

The Marketing Lead controls marketing budget and activities. Marketing can influence qualified pipeline, customer activation, revenue, and contribution. Finance owns recognized revenue and company P&L, and sales/product share responsibility for conversion and retention.

## Revenue bridge

- Completed GMV = 40,000 transactions × €3,000 = €120M.
- Transaction revenue = GMV × 5% effective fee = €6M.
- Recognized subscription revenue = 500 paid suppliers × €300 × 12 = €1.8M.
- Platform revenue = €7.8M; gross profit = €7.8M × 75% = €5.85M.
- Baseline operating expenses = €2M marketing + €1.2M sales + €1.1M product/engineering + €0.7M G&A = €5M.
- Operating profit = €850K.

## Marketing pilot and ROI

The `Pilot ROI` worksheet models a **proposed additional** €100K campaign with hypothetical incremental revenue of €180K and 75% gross margin. The base case generates €135K incremental gross profit and **35% gross-profit-based ROI** before incremental sales or other operating costs. The company P&L bridge therefore shows a hypothetical €35K operating profit uplift if all other costs remain constant.

This is **not an observed result**. It assumes the incremental revenue is genuine, collectible and can be fulfilled at the assumed incremental margin. A real-life decision should require a holdout, geo test, or another suitable incrementality method, plus sales-capacity and contribution-cost checks.

## Funnel warnings

Lead and account counts in the activity funnel are planning estimates. **Do not sum channel-sourced leads and claim unique customers unless deduplicated by account.** Funnel counts and the company revenue baseline are not mechanically linked: the model shows planning logic alongside aggregate financial context and a separate pilot P&L sensitivity, not a claim that particular channels generated €7.8M.

## Financial limitations

No taxes, interest, depreciation, working capital, FX remeasurement, deferred revenue rollforward, or detailed customer cohorts. Cost of revenue is represented by a 25% blended assumption. The model uses agent accounting for transactions. A formal company P&L would need finance-approved accounting policies and source systems.

## Decision workflow

1. Set budget and expected activation by channel.
2. Assess channel economics and capacity constraints.
3. Define an **incremental** test and success threshold before launch.
4. Track leading signals weekly; report commercial results monthly.
5. Reallocate based on **incremental contribution and confidence**, not only last-click conversions.
