# NexaDistrib International | Global Supply Chain Intelligence

### $24.83M in Revenue. 84 Stockouts. One Connected Supply Chain Story.

**SQL Server | Power BI Reporting | Supply Chain Analytics | Business Intelligence**

![NexaDistrib Supply Chain Analytics Dashboard](Thumbnail%20dashboard.png)

---

## Executive Overview

**Strong revenue doesn't always mean a healthy supply chain.**

Behind every successful distribution network lies a complex relationship between suppliers, inventory, warehouses, customer demand, and delivery operations.

This project explores a critical business question:

> **How can a global distribution business identify operational risks, improve supply chain visibility, and make smarter decisions using data?**

Using SQL Server analytics and executive-style dashboard reporting, I investigated supplier reliability, inventory shortages, warehouse capacity, revenue patterns, and delivery performance.

The objective was not simply to report operational metrics, but to connect them with business decisions.

**Project Type:** Fictional business analytics case study designed to demonstrate analytical problem-solving and executive reporting.

---

## Executive KPI Snapshot

| Business KPI | Dashboard-Reported Value | Business Significance |
|---|---:|---|
| Total Revenue | **$24.83M** | Overall reported sales performance |
| Total Orders | **58,742** | Transaction and order activity |
| Profit Margin | **17.6%** | Reported profitability |
| On-Time Delivery | **91.3%** | Delivery reliability indicator |
| Inventory Units | **1,245,780** | Reported inventory availability |
| Stockout Products | **84** | Potential replenishment risk |
| Low-Stock Products | **156** | Items requiring inventory monitoring |
| Warehouse Utilization | **72%** | Warehouse capacity usage |
| Supplier On-Time Performance | **76%** | Procurement reliability indicator |
| Late Deliveries | **36** | Reported supplier delivery exceptions |

> **Data transparency:** These figures are taken from dashboard visuals and have not been independently reconciled against the complete source dataset. They should be treated as reported indicators rather than independently verified operational results.

---

## 01 | The Business Challenge

### A Distribution Network with Multiple Operational Blind Spots

Revenue alone cannot explain whether supply chain operations are efficient.

A business may generate substantial sales while simultaneously experiencing supplier delays, inventory shortages, uneven warehouse capacity, and inconsistent delivery performance.

For NexaDistrib, this simulated analytical investigation focused on four operational questions:

1. **Procurement:** Which suppliers might be creating replenishment delays?
2. **Inventory:** Which products require urgent stock monitoring?
3. **Warehousing:** Is inventory capacity being utilized effectively?
4. **Logistics:** How reliably are orders reaching customers?

**The analytical goal:** Connect fragmented business activities into a consolidated view that helps management recognize operational risks and evaluate improvement opportunities.

---

## 02 | My Analytical Approach

### Turning Operational Data into Business Intelligence

I structured the analysis around three stages.

### Step 1 — Understand and Connect the Data

Examined relational data covering:

- Suppliers and purchase orders
- Products and inventory
- Warehouses and capacity
- Customers and sales orders
- Shipments and delivery activity

SQL joins and aggregations supported comparisons across related operational entities.

### Step 2 — Investigate Business Performance

Applied SQL Server techniques including:

| Technique | Analytical Purpose |
|---|---|
| JOINs | Connect operational entities |
| CTEs | Organize multi-stage analytical queries |
| CASE | Classify stock and delivery conditions |
| LAG() | Compare monthly revenue performance |
| RANK() | Identify leading revenue contributors |
| NTILE() | Segment customers by revenue |
| PERCENTILE_CONT() | Analyze median fulfillment duration |
| DATEDIFF() | Calculate operational time intervals |
| NULLIF() | Support safer calculations |

### Step 3 — Communicate Findings

Organized the analytical narrative into four executive dashboard areas:

**Executive Summary:** Revenue, orders, profitability, and high-level service performance.

**Inventory & Warehouse:** Stock availability, reorder points, utilization, and product-level inventory exposure.

**Supplier & Procurement:** Purchase orders, supplier reliability, and procurement performance.

**Sales & Delivery:** Customer revenue contribution, order fulfillment, and logistics performance.

---

## 03 | What the Dashboard Revealed

### Four Signals Behind Supply Chain Performance

### Insight 01 — Supplier Reliability Deserves Attention

**76% — Reported Supplier On-Time Performance**

The dashboard indicates that supplier delivery reliability may require management attention.

Inconsistent supplier timeliness can create uncertainty around replenishment schedules and product availability.

**Business implication:** Procurement teams may need to examine delays by supplier, product category, and purchase-order history.

**Recommended action:** Review recurring late deliveries and evaluate supplier-level performance before considering changes to vendor allocation.

### Insight 02 — Inventory Availability Is a Critical Risk Area

**84 Stockout Products | 156 Low-Stock Products**

The dashboard highlights products potentially facing availability constraints.

Inventory shortages can complicate order fulfillment, particularly when demand is concentrated in specific products or regions.

**Business implication:** Replenishment priorities should reflect stock levels, reorder thresholds, and sales demand.

**Recommended action:** Establish regular reorder-point reviews and prioritize products with the strongest evidence of replenishment urgency.

### Insight 03 — Warehouse Capacity Requires Closer Analysis

**72% — Reported Warehouse Utilization**

Overall warehouse utilization provides a useful starting point, but a single average cannot reveal differences between locations.

One warehouse may have spare capacity while another experiences local constraints.

**Business implication:** Warehouse-level comparisons may reveal opportunities to review capacity planning and inventory distribution.

**Recommended action:** Analyze utilization by warehouse alongside regional sales demand before proposing stock transfers.

### Insight 04 — Delivery Metrics Need Reliable Definitions

**91.3% — Reported On-Time Delivery**

Delivery performance is a major indicator of customer service quality.

However, a shipment being marked *Delivered* does not necessarily mean it arrived on time.

**Business implication:** Management decisions based on delivery KPIs require consistent measurement definitions.

**Recommended action:** Recalculate carrier performance by comparing actual delivery dates with estimated or promised dates for eligible shipments.

The reported percentage requires validation before being interpreted as a verified on-time delivery rate.

---

## 04 | From Insights to Business Decisions

### Recommended Management Priorities

| Priority | Operational Focus | Proposed Action | KPI to Monitor |
|---|---|---|---|
| High | Supplier reliability | Investigate recurring supplier delays | Supplier On-Time % |
| High | Inventory availability | Review critical reorder-point exceptions | Stockout and Low-Stock Counts |
| High | Delivery performance | Validate delivery timeliness by carrier | Verified On-Time Delivery % |
| Medium | Warehouse efficiency | Compare capacity usage against regional demand | Warehouse Utilization % |
| Medium | Customer concentration | Monitor dependency on major customers | Top-Customer Revenue Share |
| Medium | Slow-moving inventory | Review stock levels against sales activity | Inventory Turnover / Aging |

**These are proposed recommendations, not implemented operational improvements.**

---

## 05 | Dashboard Gallery

### Executive Summary Dashboard

![Executive Summary Dashboard](page%201.png)

### Inventory & Warehouse Analysis

![Inventory and Warehouse Dashboard](page%202.png)

### Supplier & Procurement Performance

![Supplier and Procurement Dashboard](page%203.png)

### Sales & Delivery Performance

![Sales and Delivery Dashboard](page%204.png)

---

## 06 | Technology Stack

| Technology | Application |
|---|---|
| SQL Server | Relational querying and operational analysis |
| T-SQL | Business logic, aggregations, and KPI calculations |
| CTEs | Structured analytical workflows |
| Window Functions | Ranking, segmentation, and trend comparisons |
| Power BI Reporting | Dashboard-based communication of analytical results |
| CSV Data | Operational source extracts |
| PowerPoint / PDF | Executive reporting and project presentation |

---

## 07 | Project Deliverables

The repository contains the following supporting materials:

| Deliverable | File |
|---|---|
| SQL Analysis | [NexaDistrib.sql](NexaDistrib.sql) |
| Dashboard Overview | [Thumbnail dashboard.png](Thumbnail%20dashboard.png) |
| Executive Dashboard | [Page 1](page%201.png) |
| Inventory Dashboard | [Page 2](page%202.png) |
| Procurement Dashboard | [Page 3](page%203.png) |
| Sales & Delivery Dashboard | [Page 4](page%204.png) |
| Business Report | [PDF Report](Global%20Supply%20Chain%20Performance%20%26%20Optimization%20Analytics.pdf) |
| Executive Presentation | [PowerPoint](Global%20Supply%20Chain%20Performance%20%26%20Optimization%20Analytics.pptx) |

---

## 08 | Analytical Limitations & Future Improvements

This portfolio case study has several important limitations:

- Dashboard figures have not been fully reconciled against the underlying source data.
- The reviewed repository did not contain an editable `.pbix` file.
- Some dimension-table source files required by SQL queries were not available among the reviewed repository assets.
- Database names require standardization across the SQL script.
- Carrier on-time calculations require correction to distinguish completed shipments from on-time deliveries.
- Full reproduction requires a complete schema, source data, and validated import process.

Future improvements include adding the missing source tables, a KPI dictionary, SQL validation checks, and the original Power BI report file if available.

---

## 09 | Skills Demonstrated

- Translating supply chain challenges into analytical business questions
- Relational SQL analysis and advanced window functions
- Operational KPI design and interpretation
- Supplier and procurement performance evaluation
- Inventory and warehouse risk analysis
- Revenue and customer segmentation
- Shipment performance analysis
- Evidence-based business recommendations
- Executive-level data storytelling and reporting

---

## Final Business Takeaway

### Revenue Tells You How Much You Sell. Operations Reveal How Reliably You Can Deliver.

The NexaDistrib case study demonstrates how connected operational analysis can help business leaders look beyond headline revenue and investigate risks across procurement, inventory, warehousing, and distribution.

The most valuable outcome of this project is the analytical framework: turning operational data into questions, investigating performance indicators, identifying potential risks, and communicating practical next steps.

**My approach: Analyze the evidence. Explain the business impact. Recommend the next decision.**

---

**Khurram Naveed | Data Analyst**

[GitHub](https://github.com/khurraminsights) · [LinkedIn](https://www.linkedin.com/in/khurram-naveed-0083851aa/)

*This project is an independent portfolio simulation and does not represent an employer engagement or a verified production deployment.*
