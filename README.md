# NexaDistrib International | Supply Chain Performance & Operations Analytics

**Portfolio Case Study | SQL Server (T-SQL) | Power BI Reporting | Supply Chain Analytics**

![Supply Chain Analytics Dashboard](Thumbnail%20dashboard.png)

## Executive Summary

This data analytics portfolio case study examines supplier reliability, inventory availability, sales trends, order fulfillment, warehouse capacity and shipment timeliness for a fictional distribution-business scenario. I used SQL Server analysis to translate operational data into actionable KPIs, and documented findings through dashboard screenshots, a PDF report and a presentation.

**Goal:** demonstrate business problem-solving, relational SQL, analytical KPI design, interpretation and stakeholder-focused reporting.

> **Scope and limitations:** NexaDistrib is presented as a portfolio case study, not evidence of employment or a production deployment. Numerical results shown in existing visuals should be validated against source data. Suggested improvements are recommendations, not independently verified achieved business outcomes.

## Business Questions

1. Which suppliers deliver purchase orders on time?
2. Which product/warehouse records indicate low or zero stock?
3. What are average and median order fulfillment times?
4. How is monthly delivered-order revenue changing?
5. Which customers contribute most to revenue?
6. Which warehouses have high or low utilization?
7. How do carriers compare on shipment timeliness?
8. Which products have low recorded sales relative to stock?

## Technical Stack

| Area | Tools and methods |
|---|---|
| SQL analytics | SQL Server, T-SQL, joins, CTEs, CASE, aggregations |
| Advanced SQL | `LAG`, `RANK`, `NTILE`, `PERCENTILE_CONT`, `DATEDIFF`, `NULLIF` |
| Data model | Related supplier, product, order, customer, warehouse and shipment entities |
| Reporting | Dashboard screenshots, presentation, PDF report |
| Data | CSV extracts for products, sales orders, purchase orders, shipments and regions |

## Analytical Workstreams

| Workstream | Analytical approach | Business value |
|---|---|---|
| Supplier reliability | Conditional counts of on-time received purchase orders | Identify suppliers needing review |
| Stock risk | Compare on-hand quantities to reorder points | Prioritize replenishment |
| Fulfillment | Average and median days from order to delivery | Understand service performance |
| Revenue | Monthly delivered-order revenue with `LAG()` | Measure month-over-month movement |
| Customer segmentation | Revenue ranking and `NTILE(4)` | Understand revenue concentration |
| Warehouse utilization | Available units divided by capacity | Identify capacity imbalance |
| Carrier performance | Compare actual to estimated delivery | Evaluate on-time service |
| Slow-moving stock | Product sales activity vs on-hand stock | Identify stock for further review |

### Selected SQL Techniques

- **CTEs** break analysis into readable stages for inventory classification, sales trends and customer revenue.
- **Window functions** rank customers and compare current-month revenue with preceding months.
- **Conditional aggregation** measures supplier delivery timeliness.
- **Date functions** calculate fulfillment durations.
- **Defensive calculations** such as `NULLIF` help avoid division-by-zero errors.

See the [original SQL analysis script](NexaDistrib.sql) for the eight complete analytical sections.

## Business Findings and Recommendations

The existing dashboard/report narrative highlights supplier delivery variation, low-stock exposure, warehouse capacity imbalance, customer concentration and differences between carriers. The following recommendations are **proposed actions**, not confirmed operational outcomes.

| Priority | Recommendation | KPI to monitor |
|---|---|---|
| High | Review delayed suppliers and evaluate vendor allocation | Supplier on-time receipt % |
| High | Apply reorder-point monitoring and replenish critical items | Out-of-stock and low-stock counts |
| High | Compare carriers using actual and estimated arrival dates | Shipment on-time % |
| Medium | Review stock redistribution against regional demand | Warehouse utilization % |
| Medium | Track major customers and diversify revenue sources | Top-customer revenue share |
| Medium | Examine unsold and slow-moving inventory | Inventory turnover / inventory aging |

## Dashboard Screenshots and Deliverables

The repository includes dashboard images and executive reporting materials:

- [Dashboard cover](Thumbnail%20dashboard.png)
- [Dashboard page 1](page%201.png)
- [Dashboard page 2](page%202.png)
- [Dashboard page 3](page%203.png)
- [Dashboard page 4](page%204.png)
- [Business report](Global%20Supply%20Chain%20Performance%20%26%20Optimization%20Analytics.pdf)
- [Presentation](Global%20Supply%20Chain%20Performance%20%26%20Optimization%20Analytics.pptx)

**Note:** No editable `.pbix` dashboard file was found in the reviewed repository. Images document the dashboard design, but do not by themselves allow the report to be run or reproduced.

## Repository Structure

```text
NexaDistrib.sql
Products.csv
Purchase_Orders.csv
Sales_Orders.csv
Shipments.csv
Regions.csv
Thumbnail dashboard.png
page 1.png
page 2.png
page 3.png
page 4.png
Global Supply Chain Performance & Optimization Analytics.pdf
Global Supply Chain Performance & Optimization Analytics.pptx
README.md
```

## How to Reproduce the Analysis

1. Download the data files and open SQL Server Management Studio.
2. Create and populate the relevant tables, including missing referenced dimension tables if you have their source files.
3. Review the SQL database context: `NexaDistrib.sql` creates `NexaDistrib` but later selects `SupplyChainDB`. Use the database where the tables were loaded.
4. Run and validate each of the eight analytical sections separately. Check join cardinality, missing dates and record counts.
5. **Carrier KPI correction needed:** the current carrier query counts `ShipmentStatus = 'Delivered'` as on time. For genuine on-time performance, use an actual-versus-estimated arrival date comparison and clearly define eligible shipments.
6. Recalculate dashboard KPIs from the complete input data before citing them as verified findings.

**Reproducibility limitation:** The SQL references `Suppliers`, `Inventory`, `Customers` and `Warehouses`, but corresponding CSV files and a complete database-import script were not found among the reviewed root-level repository files. Some queries cannot be fully reproduced from the supplied assets alone. The SQL code remains unchanged in this README-only revision.

## Skills Demonstrated

- SQL joins, CTEs, aggregations, ranking and time-series comparisons
- Operational KPI design and dimensional business analysis
- Supply chain, procurement, inventory and logistics diagnostics
- Data quality checks and transparent analytical assumptions
- Communicating findings and actionable recommendations to business audiences

## Future Improvements

- Include the missing dimension tables and a reproducible schema/import script.
- Standardize the database name in SQL.
- Correct and validate carrier delivery performance calculations.
- Add an explicit KPI dictionary and source-to-dashboard reconciliation.
- Include the original `.pbix` file if available and safe to share.

---

**Khurram Naveed | Data Analyst**  
[GitHub](https://github.com/khurraminsights) · [LinkedIn](https://www.linkedin.com/in/khurram-naveed-0083851aa/)

