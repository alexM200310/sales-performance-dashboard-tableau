# Executive Summary

## Project Overview

This project analyzes sales, profit, and quantity performance across product categories and time to identify revenue drivers, margin risks, and underperforming subcategories using Tableau.

## Key Objectives

- Track overall sales, profit, and quantity performance year-over-year
- Identify which subcategories drive revenue growth vs. which erode profit
- Visualize sales and profit trends over time to detect seasonality and volatility
- Deliver an interactive dashboard for ongoing performance monitoring

## Methodology

Sales data was loaded into Tableau and structured to support three KPI summary cards (Total Sales, Total Profit, Total Quantity), a subcategory-level sales-vs-profit comparison, and a weekly sales/profit trend view. All current-year figures are compared against the prior year across every view in the dashboard (see `tableau/Sales Dashboards.twbx`).

## Key Findings

**Sales growth is outpacing profit growth.** Total Sales grew 20.4% year-over-year to $733K, while Total Profit grew only 12.5% to $93K. Quantity sold grew fastest at 26.8%. Since units and sales are both growing faster than profit, the business is likely selling more at thinner margins rather than gaining pricing power.

**A handful of subcategories are generating sales without generating profit.** In the subcategory view, Tables shows a meaningful sales bar but a net loss in the profit chart, while Machines shows only a marginal profit despite moderate sales volume. This means revenue rank and profit rank are not the same ranking, and category strategy should be set separately for each.

**Phones, Chairs, and Copiers are the strongest combined sales-and-profit performers.** These subcategories show both high sales volume and solid green (profit-positive) bars, making them the most reliable current revenue base rather than a volatility risk.

**Weekly sales and profit are volatile but trending upward late in the year.** The weekly trend view shows frequent red (below-average) weeks earlier in the year, shifting toward more consistent green (above-average) weeks in the back half — consistent with the 20%+ annual sales growth, but suggesting performance is not evenly distributed across the year.

**Profit swings more sharply than sales on a weekly basis.** The profit trend line shows deeper relative drops and spikes than the sales trend line, meaning weekly profit is more sensitive to mix or discounting than weekly sales volume is.

## Recommendations

**Investigate margin compression before scaling volume further.** Since quantity (+26.8%) and sales (+20.4%) are both growing faster than profit (+12.5%), determine whether discounting, product mix, or cost increases are driving the gap before pushing more volume through the same channels.

**Set subcategory strategy by profit contribution, not sales volume alone.** Subcategories like Tables that show sales but negative profit should be reviewed for pricing or cost issues rather than treated as growth wins; subcategories like Phones and Copiers that are strong in both dimensions are better candidates for continued investment.

**Use Phones, Chairs, and Copiers as the current core revenue base.** These categories show durable sales-and-profit alignment and are lower-risk targets for inventory prioritization and marketing spend.

**Smooth performance across the year rather than relying on late-year strength.** Since early-year weeks trend below average and late-year weeks trend above average, evaluate whether early-year promotions or demand-generation could reduce the reliance on a strong Q4-style finish.

**Monitor weekly profit volatility separately from sales volatility.** Because profit swings more sharply week-to-week than sales, build a recurring check on discounting and cost per unit at the weekly level rather than only reviewing profit at a monthly or annual grain.

**Treat this as a single fiscal year snapshot.** The dashboard compares one year against the prior year; a future iteration should incorporate multiple years of history if the business wants to distinguish a genuine seasonal pattern from a one-year anomaly.
