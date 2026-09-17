# Retail Sales Performance Dashboard

An Excel-based analysis of 3 years (2022–2024) of retail transaction data, covering data cleaning, an interactive sales dashboard, and inventory-planning recommendations.

## What This Project Does

- Cleans and standardizes ~6,150 raw retail transaction records — removing duplicates, normalizing inconsistent category labels (e.g. "electronics" / "ELECTRONICS" / "Electronic"), and handling missing values
- Builds an interactive dashboard to track **revenue, profit margin, and order volume** across regions, product categories, and time periods
- Identifies the lowest-margin product category and seasonal demand patterns
- Summarizes findings into a one-page set of inventory-planning recommendations

## Key Finding

**Furniture** generates the highest raw revenue of any category but converts it to profit at roughly **half the rate** (16.1% margin) of top performers like Beauty & Personal Care (52%) and Apparel (48%) — pointing to a supply-chain/landed-cost issue rather than a demand problem.

Revenue also shows a clear seasonal pattern, peaking ~55–60% above baseline in November–December.

## Tech / Approach

- **Data cleaning**: deduplication, category label standardization, missing-value imputation (category median for numeric fields, "Unspecified" flag for missing region)
- **Dashboard**: dropdown filters (Region / Category / Year) driving live KPI cards and charts, built with `SUMIFS` / `COUNTIFS` formulas — a formula-driven equivalent of native PivotTables + Slicers
- **Charts**: revenue by category, monthly revenue trend, revenue share by region, order volume by category

## File Structure

| Sheet | Contents |
|---|---|
| `Raw Data` | Original unprocessed transaction export |
| `Cleaned Transactions` | Standardized dataset (Excel Table) |
| `Dashboard` | Interactive filters, KPIs, and charts |
| `Insights & Recommendations` | One-page summary + data cleaning log |

## How to Use

1. Download `Retail Sales Performance Dashboard.xlsx`
2. Open in Excel and enable editing
3. Go to the **Dashboard** tab and use the Region / Category / Year dropdowns to filter — KPIs, tables, and charts update live
