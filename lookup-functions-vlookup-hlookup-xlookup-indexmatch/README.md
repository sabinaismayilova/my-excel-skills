# Excel Lookup Functions — VLOOKUP, HLOOKUP, XLOOKUP, INDEX/MATCH

A practice workbook demonstrating four core Excel lookup approaches on a
retail sales dataset (10,000-row order table).

## What's inside

- **Task 1 — VLOOKUP**: pulls order-level details (date, segment, city,
  region, ship mode, customer ID) from a raw data table by Order ID.
- **Task 2 — HLOOKUP**: retrieves revenue from a horizontally-laid-out
  lookup table, using exact match mode.
- **Task 3 — XLOOKUP**: looks up ship mode by Order ID, with a
  "not found" fallback for unmatched values.
- **Task Set 2 — MIN / MATCH / INDEX**: finds the lowest-cost day of the
  week for each phone number and returns both its position and its name.

## Skills demonstrated

- Exact-match lookups (`FALSE` / `0`) vs. Excel's default approximate match
- Absolute (`$`) vs. relative cell referencing, and why it matters when
  copying formulas down a column
- Combining `INDEX` and `MATCH` to return a label rather than a value
- Building a fallback / error-handling argument into a lookup formula

## Compatibility note

`XLOOKUP` requires Excel 365 or Excel 2021+; it will not calculate in
older Excel versions, Google Sheets, or LibreOffice. `VLOOKUP`,
`HLOOKUP`, and `INDEX/MATCH` work everywhere.

## File

`lookup-functions-vlookup-hlookup-xlookup-indexmatch.xlsx`
