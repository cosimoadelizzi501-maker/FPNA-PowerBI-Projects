# Enterprise Sales Performance & Variance Analytics (Actual vs Budget)

## Executive Overview
This project provides an end-to-end sales performance and variance analysis framework designed for corporate finance and commercial controlling. Integrating a relational SQL database with an executive Power BI reporting model, it enables commercial leaders to track actual revenue against budget targets across product lines, evaluate pricing trends, and assess product-level contribution margins.

---

## Tech Stack & Data Architecture
* **Relational Database (SQL):** ANSI / SQLite schema design
  * Dimensions: `Prodotti` (Product catalog, business lines, standard unit costs)
  * Facts: `Vendite_Dettaglio` (Actual sales transactions, volume, unit prices, revenues, total costs)
  * Budgets: `Budget_Vendite` (Monthly sales targets by product)
  * Analytics Views: `vw_Vendite_Marginalita` (Relational joins and automated gross margin calculation)
* **BI Engine & Modeling:** Power BI Desktop
  * Normalized Star Schema design with 1:N relationships
  * Dedicated Date/Time dimensions for temporal aggregation
* **Calculations & DAX:**
  * Actual vs Budget absolute variance: `[Ricavi Actual] - [Ricavi Budget]`
  * Percentage variance and target achievement metrics
  * Dynamic conditional formatting logic for variance alerts

---

## Key Business Insights Delivered
* **Variance Analysis:** Instant identification of revenue gaps versus targets across Corporate and Retail lines.
* **Margin Tracking:** Real-time visibility on product profitability and cost-to-revenue ratios.
* **Executive Decision-Making:** Interactive slicers and visual alerts enabling quick root-cause diagnosis on underperforming product categories.

---

## Repository Structure
* `Progetto_Enterprise_Sales_Dashboard.pbix`: Full interactive Power BI data model and executive dashboard.
* `fpna_sales_model.sql`: Complete DDL/DML script with tables, seed datasets, and analytical view.
* `Progetto_Enterprise_Sales_Dashboard.pdf`: Executive-ready reporting export.
* 
