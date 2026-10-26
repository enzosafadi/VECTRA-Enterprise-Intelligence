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

## Repository packaging checks — 26 October 2026
- XLSX ZIP integrity: passed; workbook readable programmatically; 19 worksheets present.
- Detailed finance: 48 records, 12 plants × four months (January–April 2026).
- Independent source calculations: revenue CAD 32,665,304; operating profit CAD 7,576,492; margin 23.1943%; weighted on-time delivery 87.5900%. Rendered cockpit values match these spot checks.
- Scenario and executive KPI ranges rendered and visually inspected. This is not desktop Excel acceptance or comprehensive formula testing.
- One canonical workbook; documentation and image paths checked in the repository tree.

### Additional known defects / follow-up
- Annual labels describe four-month totals; correct labels before the final release.
- Map label placement and city-coordinate association need verification before final publication.
- Fixed formula ranges require review when rows are added.
- Desktop Excel repair warnings, interactive behavior, chart rendering and full reconciliation remain untested.

Workbook SHA-256: `847dfd6d3c6ce0f4de792911a5d697c9536779d5ba1ed2be6074f68e152578c4`.
