# VECTRA — User Manual
**Version 0.5 · 26 October 2026 · Development edition**

All business data are synthetic. This workbook is a portfolio demonstration, not an operational ERP or audited financial system.

## Quick start
1. Open `VECTRA_Enterprise_Intelligence_v0.5_Enterprise.xlsx` in desktop Microsoft Excel.
2. Enable editing if appropriate. **Do not enable macros:** this edition contains no VBA.
3. Begin with **START HERE**, then **EXECUTIVE COCKPIT**.
4. Review the data modules to investigate plant-level exceptions.
5. Save a working copy before changing assumptions or source records.

## Worksheet reference
| Worksheet | What it does | Operator action |
|---|---|---|
| START HERE | Workbook orientation | Follow the workflow |
| EXECUTIVE COCKPIT | Formula-driven network KPIs | Review targets, exceptions and chart |
| FINANCE DATA | Plant-month P&L | Inspect costs, margins and profitability |
| OPERATIONS DATA | Yield, delivery and capacity | Investigate late orders and downtime |
| WORKFORCE DATA | Shift staffing | Review coverage and overtime flags |
| INVENTORY DATA | Replenishment alerts | Compare on-hand units and reorder points |
| ISSUE REGISTER | Risk ownership | Maintain owner, status and mitigation |
| SCENARIO ENGINE | Financial sensitivities | Select Base/Downside/Upside in column E |
| GEO INTELLIGENCE | Facility geographic dataset | Filter site metrics |
| PLANT NETWORK MAP | Geographic snapshot | View static map image |
| CONTROL CENTER and original sheets | Earlier demo dashboards | **Do not reconcile with detailed dataset** |

## Safe editing
**Editable:** `SCENARIO ENGINE!E4:E7` dropdowns; issue status and descriptive mitigation fields; simulated source inputs when testing a copy.

**Preserve formulas:** `FINANCE DATA!H:J`, `OPERATIONS DATA!K:M`, `WORKFORCE DATA!H:I`, `INVENTORY DATA!J:K`, `ISSUE REGISTER!G`, `EXECUTIVE COCKPIT!B4:B12`, and `SCENARIO ENGINE!B11:B16`.

## Example management workflow
A director notices deteriorating delivery performance in **EXECUTIVE COCKPIT**. Filter **OPERATIONS DATA** by plant and month, inspect delays/downtime, check **WORKFORCE DATA** for staffing gaps, compare **INVENTORY DATA** reorder alerts, document mitigation in **ISSUE REGISTER**, and test a cost/revenue sensitivity in **SCENARIO ENGINE**.

## Scenario analysis
Choose the desired case in `SCENARIO ENGINE` column E for each modeled driver. Revenue, material, labor, overhead, profit and margin estimates recalculate from detailed finance data. These are directional sensitivities, **not probability-weighted forecasts**.

## Mapping
The workbook currently embeds a **static** Canadian plant map. For an interactive Excel tour, use desktop Excel **Insert → 3D Map** with plant, latitude, longitude and a numeric metric. A 3D Maps tour is **not included** in v0.5.

## Troubleshooting
- **Excel asks to repair workbook:** do not ignore; retain a copy and report the message.
- **Formulas show old results:** set calculation to Automatic and recalculate.
- **Map does not move/filter:** expected; it is an image.
- **Totals disagree across older and newer tabs:** expected because the datasets are not reconciled.
- **Charts look different:** verify in desktop Excel before publishing screenshots.

## Publishing and acceptance
Complete the checks in [VALIDATION.md](VALIDATION.md). Capture genuine screenshots from Excel only after verification. Do not claim Power Query, VBA, slicers, 3D Maps or enterprise deployment until actually implemented.

## Reporting period and current release caveats
The detailed finance model contains January–April 2026 only. The cockpit's “Annual revenue” and “Annual operating profit,” and the scenario engine's “MODELED ANNUAL P&L,” actually sum these four months. Do not interpret them as full-year or annualized amounts. The workbook has been preserved unchanged in this publication.

Scenario selections are independent for each driver; a mixed selection is a hybrid sensitivity. Formula ranges are fixed: appending rows does not guarantee that summary formulas expand. Check every affected reference after extending a dataset.

The map and older dashboard tabs use a separate synthetic sample. Map status colors and bubble sizes should not be compared with the detailed cockpit totals. See the [preview provenance](../assets/README.md).
