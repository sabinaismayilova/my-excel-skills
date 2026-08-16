# IF/AND/OR Logic, Histogram & Box-and-Whisker Analysis

A workbook covering nested conditional logic and statistical charting,
applied to a 10,000-row retail order dataset.

## What's inside

**IF_AND_OR sheet:**
- An 11-bracket nested IF/AND formula categorizing every order's Declared
  Revenue into ranges (0–1 AZN, 1–3 AZN, ... up to 1000–2000 AZN)
- A combined AND/OR condition flagging orders for a company audit: orders
  from a specific city (Los Angeles) OR any order with Declared Revenue
  above 1700 AZN, regardless of city
- Two cross-tabulated summary tables (Order Count and Total Declared
  Revenue, both filtered to audited orders only) broken out by Product
  Category × Segment

**Stat_Viz sheet:**
- A Histogram of Total Revenue with a fixed bin width (100 AZN) and a
  manually defined overflow bucket (>1000 AZN)
- A Box-and-Whisker chart comparing Sales Quantity distribution across
  three customer segments (Consumer, Corporate, Home Office)
- Written statistical interpretation covering skew, median vs. mean, and
  outlier patterns, backed by calculated quartiles (Q1, Q3, IQR) and
  outlier thresholds (1.5 × IQR) for each segment

## Skills demonstrated

- Nested IF statements combined with AND/OR logic for multi-condition
  categorization and flagging
- Structuring SUMIFS/COUNTIFS formulas for cross-tabulated tables using
  mixed absolute/relative references, so one formula copies correctly
  across both rows and columns
- Choosing the right chart type for the question being asked (Histogram
  for distribution shape, Box-and-Whisker for comparing spread and
  outliers across groups)
- Calculating and interpreting median, mean, quartiles, IQR, and outlier
  thresholds — and explaining why mean and median diverge when a
  distribution is skewed by outliers

## File

`if-and-or-histogram-boxplot.xlsx`
