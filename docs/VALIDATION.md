# VECTRA — Validation and Release Gate

**Current release:** v0.5, development. **Desktop acceptance: not yet performed.**

## Acceptance checklist
- [ ] Workbook opens in desktop Excel **without repair warnings**.
- [ ] Every expected worksheet is present and legible at normal zoom.
- [ ] Automatic calculation and formulas produce consistent results.
- [ ] Executive cockpit totals reconcile to **detailed** source sheets.
- [ ] Scenario dropdowns update the relevant outputs.
- [ ] Issue status validation and risk scores behave correctly.
- [ ] Inventory alerts respond to changed stock levels.
- [ ] Workforce exceptions respond to changed shift inputs.
- [ ] Plant map image displays at intended dimensions.
- [ ] No broken references, unexpected `#REF!`, `#DIV/0!` or `#VALUE!` errors.
- [ ] Screenshots captured from the actual verified Excel workbook.

## Known limitations
1. Older sheets and v0.5 detailed data are separate synthetic samples, not a reconciled ledger.
2. The geographic map is an embedded image, not an interactive Excel 3D Map.
3. No Power Query pipeline, Power Pivot model, PivotTable slicers or VBA is included.
4. No production-grade scheduling optimization, audit trail, access controls or live integrations.
5. Visual QA in desktop Excel and complete cross-module reconciliation remain outstanding.

**Release rule:** Do not label the workbook enterprise-ready or Upwork-final until these gates are passed.
