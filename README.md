# Tableau Sales Dashboard

An interactive Tableau dashboard analyzing sales performance, profitability, and product trends to identify growth drivers and underperforming categories.

**Live Dashboard:** [View on Tableau Public](https://public.tableau.com/views/SalesCustomerDashboards_17870875614940/SalesDashboard?:language=en-US&publish=yes&:showVizHome=no)

## Repository Structure

```
tableau-sales-dashboard/
├── data/
│   └── raw/              # Raw source data (CSV files)
├── tableau/
│   ├── Sales Dashboards.twbx   # Packaged Tableau workbook
│   └── screenshot.png          # Dashboard preview
├── README.md
└── EXECUTIVE_SUMMARY.md
```

## Project Overview

This project analyzes sales, profit, and quantity data across product categories, regions, and time to surface performance trends and inform inventory and pricing decisions.

## Key Objectives

- Track overall sales, profit, and quantity performance year-over-year
- Identify which subcategories drive revenue vs. which drive losses
- Visualize sales and profit trends over time to spot seasonality
- Allow drill-down by year, category, sub-category, and location
- Deliver an interactive, filterable dashboard for ongoing monitoring

## Dashboard Preview

![Sales Dashboard Preview](tableau/screenshot.png)

## Interactivity

The live dashboard includes a filter panel supporting:

- **Select Year** — switch the analysis year
- **Product** — filter by Category and Sub-Category
- **Location** — filter by Region, State, and City
- **Min/Max sliders** — constrain the view by Sales, Profit, and Quantity ranges

All three KPI cards and both charts respond to these filters, and the subcategory and time-series charts support drill-down on click.

## Methodology

Raw sales data was loaded into Tableau and modeled to support three KPI summary cards (Total Sales, Total Profit, Total Quantity), a subcategory-level sales/profit comparison, and a weekly sales/profit trend view. The dashboard compares current-year performance against the prior year across all views, with a full filter panel for year, product, and location.

## Key Findings

See [EXECUTIVE_SUMMARY.md](EXECUTIVE_SUMMARY.md) for the full write-up.

- Total Sales reached $733K, up 20.4% year-over-year
- Total Profit reached $93K, up 12.5% year-over-year
- Total Quantity sold reached 12K units, up 26.8% year-over-year
- Profit growth is lagging sales and quantity growth, suggesting margin pressure worth investigating
- Several subcategories (including Tables) post negative profit despite generating sales, while categories like Phones, Chairs, and Copiers show strong profit contribution

## Tools Used

- Tableau (dashboard design, visualization, and publishing to Tableau Public)

## How to Open

- **View online:** open the [live dashboard](https://public.tableau.com/views/SalesCustomerDashboards_17870875614940/SalesDashboard?:language=en-US&publish=yes&:showVizHome=no) — no software required
- **Open locally:** download `tableau/Sales Dashboards.twbx` and open with Tableau Desktop or Tableau Public
