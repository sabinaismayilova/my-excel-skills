# Math & Text Functions — COUNT, COUNTA, SUM, AVERAGE, LEFT, RIGHT, MID, SEARCH

A two-part practice workbook covering Excel's core math/logic functions
and text-parsing functions, plus a real-world application on a 10,000-row
order dataset.

## What's inside

**Math Functions sheet:**
- COUNTA vs COUNT — counting all non-empty cells vs. numeric-only cells
  in a mixed-type column (numbers, text, and a date together)
- SUM and AVERAGE on numeric ranges
- Comparison and logical operators (`>`, `<=`, `=`, `<>`) to evaluate TRUE/FALSE
  conditions, including exponents (`^`)

**Text Functions sheet:**
- LEFT, RIGHT, and MID used individually and nested inside one another
  (e.g. `RIGHT(LEFT(text,12),4)`) to extract specific substrings from a
  fixed-position source string
- Two extraction methods solved side by side (a LEFT/RIGHT approach and
  a MID approach) to arrive at the same result, showing the trade-offs
  between each

**Raw sheet (applied to real data):**
- Order IDs and Customer IDs are compound values (e.g. `"CA-2016-152156"`,
  `"CG-12520"`) — a code and a number joined by a hyphen. Rather than
  assuming a fixed character count on either side, `SEARCH("-", cell)`
  locates the hyphen's exact position in each row, and that position is
  then fed into LEFT, RIGHT, and MID to split the string apart correctly:
  - `LEFT(text, SEARCH("-",text)-1)` → everything before the hyphen
  - `RIGHT(text, LEN(text)-SEARCH("-",text))` → everything after the hyphen
  - `MID(text, SEARCH("-",text)+1, 4)` → a fixed-length chunk starting
    right after the hyphen (used to pull the 4-digit year from the
    Order ID)
- Applied consistently across ~9,994 rows to derive Order Year, Customer
  Type, and Customer Number from the original ID fields

## Skills demonstrated

- Distinguishing COUNT (numeric only) from COUNTA (any non-empty cell)
  and choosing the right one for the question being asked
- Nesting text functions to isolate a substring in more than one way
- Using SEARCH to dynamically locate a delimiter's position rather than
  hardcoding a character count, so the same formula still parses correctly
  even when the text on either side of the delimiter varies in length
  from row to row

## File

`math-text-functions-count-sum-average-left-right-mid-search-len.xlsx`
