# PivotTables

A workbook demonstrating 8 native Excel PivotTables built on a 10,000-row
retail order dataset, plus formula-based fraud detection identifying
orders where the sale price didn't match the required unit price.

## What's inside

**Task 1 (Table) sheet:**
- The raw order dataset converted into a proper Excel structured Table
  object (not just a formatted range), with auto-filter enabled — the
  standard way to prepare a dataset as a reliable, dynamically-expanding
  PivotTable source
- Five interactive Slicers (Order Date Year, Ship Mode, Segment, City,
  Region) connected to the PivotTables, letting the whole dashboard be
  filtered interactively without editing any formulas

**Raw Data sheet:**
- Four calculated columns detecting pricing discrepancies for every
  order:
  - **Actual Unit Price** — Declared Revenue ÷ Quantity, backing out
    what price was actually charged
  - **Is Price Wrong?** — flags whether that actual price differs from
    the required Unit Price
  - **Expected Revenue** — Unit Price × Quantity, what revenue should
    have been if the correct price was used
  - **Difference** — Expected Revenue minus Declared Revenue, the size
    of the pricing discrepancy on each order

**Task 2 (Execution) sheet — 8 native PivotTables:**
- Order Count, Total Quantity Sold, and Total Declared Revenue, each
  broken out by Ship Mode × Segment
- Revenue per Order, built using a PivotTable's Average subtotal on
  Declared Revenue — mathematically equivalent to dividing the Revenue
  table by the Order Count table, but computed natively in one step
- Order Count, Total Quantity Sold, and Total Declared Revenue again,
  this time broken out by Order Year × Segment
- A summary of the fraud-detection Difference values, broken out by
  Order Year × Product Category, isolating exactly where and when
  pricing discrepancies occurred


## Skills demonstrated

- Converting a raw data range into a structured Excel Table object as a
  clean, reliable PivotTable data source
- Building PivotTables from a single shared pivot cache, using multiple
  aggregation types (Sum, Count, Average) depending on the question
  being asked
- Choosing the right subtotal function to answer a derived metric in
  one step (Average) instead of building it from two separate totals
- Adding Slicers to PivotTables for interactive, click-to-filter
  exploration of the dashboard, rather than a static set of tables
- Formula-based anomaly detection: reconstructing an expected value
  from source fields and calculating the deviation from what was
  actually recorded


## File

`pivot-tables-cross-tab-summaries.xlsx`
