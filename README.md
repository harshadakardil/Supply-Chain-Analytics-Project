# Supply Chain Intelligence
## Optimizing Delivery Performance and Demand Forecasting

**Tools:** Excel | SQL | Power BI
**Domain:** Supply Chain / Logistics
**Type:** Business Analysis + Data Analytics Project
**Author:** Harshada Kardile

---

## Problem Statement
An e-commerce retailer experiencing:
- On-Time Delivery Rate of only 16.48% (target ≥ 90%)
- Logistics Cost per Order = $325.52 (reduce by 10%)
- Stockout Rate = 44.28% (target ≤ 3%)

---

## BA Approach
- Elicited 12 business requirements from 5 stakeholder groups
- Documented Requirements Traceability Matrix (RTM)
- Performed AS-IS / TO-BE gap analysis
- Defined acceptance criteria for all 8 KPIs

---

## What I Did

### Excel
- Data cleaning — duplicates, nulls, date standardization
- Calculated columns — Delivery Delay Days, Cost Per Unit
- Pivot tables — carrier and region performance summary
- Multiple Linear Regression — R²=0.173, RMSE=2.07
- Demand Forecasting — Moving Average + Exponential 
  Smoothing (α=0.3), MAPE=4.96%
- K-Means Clustering — manual elbow method, K=3 selected
  (WCSS: K1=15.4, K2=8.7, K3=4.3, K4=3.9)

### SQL
- 3-table normalized schema (Orders, Suppliers, Inventory)
- Query 1: Carrier performance — aggregation + STDDEV
- Query 2: Monthly SKU trend — rolling 3-month window function
- Query 3: Regional carrier ranking — DENSE_RANK
- Query 4: Supplier delivery performance — INNER JOIN

### Power BI
- 5-page interactive dashboard
- 8 KPIs on Executive Overview page
- 4 slicers — Region, Carrier, Product Category, Date
- Pages: Overview | Delivery | Cost | Supplier | Forecast

---

## Key Findings
| Finding | Value |
|---|---|
| Overall On-Time Rate | 16.48% |
| Best Carrier | DHL — 47.9% on-time |
| Worst Carrier | XpressBees — 0.4% on-time |
| Worst Region | Northeast — 1.3% on-time |
| Stockout Rate | 44.28% |
| Critical Suppliers | 5 of 15 |

---

## Recommendations
1. Shift volume from XpressBees to DHL on Northeast/Northwest
2. Place 5 Critical suppliers on 90-day corrective action plan
3. Recalibrate reorder points using demand forecast
4. Standardize carrier SLAs with penalty clauses
5. Monthly supplier scorecard refresh using cluster logic
6. Pilot DHL on problem routes before national rollout

---

## Project Files
| File | Description |
|---|---|
| Excel Workbook | Cleaning, analysis, RTM, forecasting, clustering |
| SQL Scripts (8 files) | Schema + 4 analysis queries |
| Power BI Dashboard | 5-page interactive dashboard |
| Report | Full BA report with AS-IS/TO-BE, RTM |
| Presentation | 20-slide deck |

---

## BA Deliverables
- Requirements Traceability Matrix (RTM) — 12 requirements
- AS-IS / TO-BE Gap Analysis
- Stakeholder Analysis — 5 groups
- Business Recommendations — prioritized by impact vs effort
