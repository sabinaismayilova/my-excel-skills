# SUMIFS, COUNTIFS & Multi-Condition Summary Tables

A practice workbook building cross-tabulated summary tables from a
10,000-row retail order dataset — using only math formulas (no
PivotTables), broken out by Ship Mode, Segment, and Order Year, with
additional filter conditions layered on top.

## What's inside

**Task Set 1 — baseline summary tables (by Ship Mode):**
- Order Count, Total Quantity Sold, and Declared Revenue, each
  broken down by Ship Mode
- Two derived ratio tables built from those results: Revenue per
  Order and Revenue per Unit
- A second set of tables breaking the same three metrics out by
  Order Year instead of Ship Mode
- Color Scale conditional formatting applied to the data cells,
  excluding totals

**Task Set 2 — the same tables with an added filter condition:**
- Order Count filtered to Order Date >= 2015
- Total Quantity Sold filtered to a specific date range
  (2015 <= Order Date < 2017)
- Declared Revenue filtered to a specific region (Delaware)

**Task Set 3 — the same six tasks again, cross-tabulated by Segment:**
- Every table from Task Set 1 rebuilt with Consumer, Corporate, and
  Home Office as separate columns, so each row/column intersection
  is its own condition (Ship Mode AND Segment, or Year AND Segment)

## Skills demonstrated

- COUNTIFS and SUMIFS with single and multiple conditions
- Structuring formulas so they copy correctly across both rows and
  columns in a cross-tab layout (mixed absolute/relative references)
- Building derived ratio metrics (per-order, per-unit) from prior
  formula results rather than recalculating from raw data
- Applying comparison operators inside SUMIFS/COUNTIFS criteria
  (>=, <, exact match, text match) to layer additional filters onto
  an existing table structure
- Color Scale conditional formatting applied selectively (data cells
  only, not totals)

## File

`sumifs-countifs-multi-condition-summary-tables.xlsx`
