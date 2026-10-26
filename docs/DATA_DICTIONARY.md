# VECTRA — Data Dictionary (v0.5)

| Dataset / worksheet | Grain | Main measures | Derived measures |
|---|---|---|---|
| FINANCE DATA | Plant × month | Revenue, materials, labor, overhead | Profit, margin, cost ratio |
| OPERATIONS DATA | Plant × month | Production, defects, orders, delivery, downtime | Yield, on-time rate, utilization |
| WORKFORCE DATA | Plant × shift | Scheduled, available staff, overtime | Coverage, exception flags |
| INVENTORY DATA | Plant × SKU | On hand, usage, lead time, safety stock | Reorder point, alert |
| ISSUE REGISTER | Individual issue | Likelihood, impact, owner, status | Risk score |
| SCENARIO ENGINE | Financial driver | Selected scenario and assumptions | Modeled revenue, cost, profit, margin |
| GEO INTELLIGENCE | Plant | Facility location and regional metrics | Geographic comparison |

**Source:** All records are fictional and intended for demonstration. Older retained dashboard sheets are not reconciled with these datasets.

**Governance:** Treat source-input cells as editable only in working copies; formula fields as protected-by-convention. No real access control is implemented.
