# Project 5: Inventory Management Analytics

## 1. Business Scenario

An operations team wants to reduce stockouts, avoid excess inventory and improve supplier reliability while keeping inventory investment under control.

Your task is to act as a **Business Data Analyst** and convert the raw operational data into a Pivot Table-based management report.

---

## 2. Dataset Overview

This project is designed to practice:

- Excel Tables
- Pivot Tables
- Pivot Charts
- Slicers
- Timeline
- KPI calculations
- Benchmark comparison
- Conditional Formatting
- Business insights
- Management decision-making

### Dataset Columns

| Column | Description |
|---|---|
| SKU | Product SKU |
| Month | Reporting month |
| Warehouse | Warehouse |
| Category | Product category |
| Product | Product name |
| Supplier | Supplier |
| Opening_Stock | Opening stock units |
| Purchases | Units purchased |
| Units_Sold | Units sold |
| Closing_Stock | Closing stock units |
| Reorder_Level | Reorder level |
| Unit_Cost | Cost per unit |
| Stockout_Days | Days product was out of stock |
| Defective_Units | Defective units |
| Lead_Time_Days | Supplier lead time |

---

## 3. Dataset

Save the following data as:

`05_inventory_management_analytics.csv`

```csv
SKU,Month,Warehouse,Category,Product,Supplier,Opening_Stock,Purchases,Units_Sold,Closing_Stock,Reorder_Level,Unit_Cost,Stockout_Days,Defective_Units,Lead_Time_Days
SKU001,2026-01,Noida,Accessories,Monitor,Supplier D,297,269,38,528,60,35579,3,0,2
SKU002,2026-02,Noida,Accessories,Router,Supplier D,462,111,84,489,177,7012,1,1,5
SKU003,2026-03,Noida,Electronics,Monitor,Supplier A,90,211,237,64,118,37727,3,11,5
SKU004,2026-04,Gurgaon,Electronics,Webcam,Supplier D,257,214,223,248,130,31895,0,10,2
SKU005,2026-05,Mumbai,Accessories,Monitor,Supplier A,380,189,319,250,169,6949,0,7,5
SKU006,2026-06,Delhi,Office,Mouse,Supplier D,400,163,308,255,132,43829,0,5,7
SKU007,2026-01,Noida,Networking,Mouse,Supplier A,89,173,113,149,132,16459,3,5,10
SKU008,2026-02,Mumbai,Accessories,Monitor,Supplier C,306,197,57,446,72,29345,1,0,7
SKU009,2026-03,Mumbai,Electronics,Router,Supplier B,451,250,281,420,89,24018,3,6,4
SKU010,2026-04,Noida,Accessories,Keyboard,Supplier A,415,57,72,400,94,10807,3,1,8
SKU011,2026-05,Delhi,Office,Headset,Supplier D,52,177,257,0,106,50595,4,1,4
SKU012,2026-06,Delhi,Accessories,Headset,Supplier A,335,282,238,379,73,2421,0,5,10
SKU013,2026-01,Gurgaon,Networking,Mouse,Supplier B,199,231,228,202,159,6250,1,9,10
SKU014,2026-02,Noida,Networking,Router,Supplier D,187,174,167,194,123,10263,0,2,8
SKU015,2026-03,Gurgaon,Networking,Keyboard,Supplier B,450,59,214,295,92,16860,3,9,11
SKU016,2026-04,Noida,Networking,Mouse,Supplier C,205,23,232,0,102,55855,6,5,9
SKU017,2026-05,Mumbai,Office,Laptop Stand,Supplier D,214,122,275,61,100,12341,6,5,6
SKU018,2026-06,Gurgaon,Electronics,Webcam,Supplier B,193,221,216,198,74,37652,1,9,10
SKU019,2026-01,Noida,Office,Router,Supplier B,274,169,384,59,68,54371,6,15,4
SKU020,2026-02,Mumbai,Networking,Monitor,Supplier C,416,236,434,218,108,5547,3,19,9
SKU021,2026-03,Noida,Office,Monitor,Supplier D,409,294,334,369,141,6269,0,7,12
SKU022,2026-04,Gurgaon,Office,Webcam,Supplier C,435,189,437,187,115,7643,0,3,6
SKU023,2026-05,Delhi,Networking,Keyboard,Supplier C,250,257,425,82,146,39273,8,4,7
SKU024,2026-06,Noida,Networking,Printer,Supplier D,262,63,89,236,166,48551,1,2,6
SKU025,2026-01,Noida,Electronics,Keyboard,Supplier A,228,263,79,412,116,48016,3,2,3
SKU026,2026-02,Gurgaon,Office,Laptop Stand,Supplier D,484,195,361,318,73,45077,1,7,10
SKU027,2026-03,Mumbai,Networking,Monitor,Supplier B,286,138,438,0,111,41971,2,5,12
SKU028,2026-04,Delhi,Electronics,Mouse,Supplier C,280,239,229,290,60,46885,1,3,6
SKU029,2026-05,Noida,Networking,Headset,Supplier A,216,120,264,72,74,17893,7,8,12
SKU030,2026-06,Delhi,Office,Laptop Stand,Supplier A,228,200,264,164,139,12006,2,9,11
SKU031,2026-01,Mumbai,Office,Headset,Supplier D,172,176,89,259,83,25164,1,4,8
SKU032,2026-02,Mumbai,Accessories,Mouse,Supplier B,145,269,355,59,128,46144,2,17,4
SKU033,2026-03,Gurgaon,Office,Headset,Supplier D,211,250,347,114,66,57422,2,0,9
SKU034,2026-04,Delhi,Electronics,Printer,Supplier C,259,271,242,288,150,55743,3,7,4
SKU035,2026-05,Mumbai,Electronics,Keyboard,Supplier C,66,160,145,81,128,19618,2,7,11
SKU036,2026-06,Gurgaon,Networking,Keyboard,Supplier B,446,298,217,527,129,54610,0,7,10
SKU037,2026-01,Gurgaon,Office,Laptop Stand,Supplier D,202,36,260,0,93,23544,1,7,3
SKU038,2026-02,Noida,Accessories,Mouse,Supplier C,134,91,431,0,86,54015,3,1,11
SKU039,2026-03,Delhi,Accessories,Mouse,Supplier B,410,169,178,401,133,18220,0,2,8
SKU040,2026-04,Gurgaon,Accessories,Headset,Supplier D,177,94,394,0,101,54995,3,12,9
SKU041,2026-05,Noida,Accessories,Webcam,Supplier D,281,58,354,0,161,58379,1,12,10
SKU042,2026-06,Noida,Electronics,Headset,Supplier B,217,21,426,0,168,48719,1,14,12
SKU043,2026-01,Gurgaon,Networking,Laptop Stand,Supplier A,269,128,283,114,94,21859,2,5,10
SKU044,2026-02,Gurgaon,Networking,Webcam,Supplier A,73,70,350,0,160,55534,7,0,3
SKU045,2026-03,Delhi,Accessories,Router,Supplier A,269,123,382,10,176,9345,4,5,6
SKU046,2026-04,Mumbai,Electronics,Keyboard,Supplier A,240,104,56,288,110,41699,2,2,5
SKU047,2026-05,Delhi,Accessories,Keyboard,Supplier D,159,264,69,354,76,39607,1,3,2
SKU048,2026-06,Delhi,Accessories,Laptop Stand,Supplier C,405,87,274,218,69,15704,3,1,3
SKU049,2026-01,Gurgaon,Electronics,Monitor,Supplier B,120,215,426,0,164,50058,2,20,12
SKU050,2026-02,Mumbai,Office,Keyboard,Supplier A,275,199,399,75,87,41861,2,13,11
SKU051,2026-03,Gurgaon,Office,Router,Supplier A,121,83,331,0,153,25867,5,13,7
SKU052,2026-04,Gurgaon,Office,Headset,Supplier C,177,165,428,0,180,45951,0,21,6
SKU053,2026-05,Delhi,Office,Webcam,Supplier A,380,47,431,0,174,52721,3,15,8
SKU054,2026-06,Mumbai,Accessories,Mouse,Supplier D,320,26,214,132,179,21440,2,6,11
SKU055,2026-01,Delhi,Electronics,Headset,Supplier C,444,57,38,463,135,5125,0,1,5
SKU056,2026-02,Gurgaon,Accessories,Keyboard,Supplier C,371,276,422,225,113,28459,3,2,12
SKU057,2026-03,Delhi,Accessories,Headset,Supplier B,90,281,134,237,163,10882,2,3,11
SKU058,2026-04,Delhi,Accessories,Mouse,Supplier A,79,145,74,150,178,29174,1,3,11
SKU059,2026-05,Noida,Office,Laptop Stand,Supplier B,56,90,389,0,61,11436,7,11,10
SKU060,2026-06,Noida,Electronics,Router,Supplier A,433,157,405,185,173,8436,0,10,8
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| Stockout Days | 2 or fewer |
| Defect Rate | 3% or lower |
| Inventory Turnover | 4× or higher |
| Supplier Lead Time | 7 days or lower |
| Closing Stock | Above Reorder Level |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **Inventory Value**: `Closing Stock × Unit Cost`
- **Defect Rate**: `Defective Units / Units Sold × 100`
- **Stockout Rate**: `SKUs with Stockout Days > 2 / Total SKUs × 100`
- **Inventory Turnover**: `Units Sold / Average Inventory Units`
- **Reorder Risk**: `Closing Stock < Reorder Level`

---

## 6. Assignment Tasks

### Task 1 — Warehouse Performance
Compare warehouses by stock value, units sold, stockout days and defect rate.
### Task 2 — Product Performance
Analyze products by units sold, closing stock, stock value and stockout days.
### Task 3 — Supplier Analysis
Compare suppliers by purchases, lead time, defective units and estimated defect rate.
### Task 4 — Reorder Risk
Identify SKUs where Closing Stock is below Reorder Level.
### Task 5 — Stockout Analysis
Find products and warehouses with the highest stockout days.
### Task 6 — Inventory Value
Calculate inventory value using Closing Stock × Unit Cost and compare categories.
### Task 7 — Monthly Trend
Analyze purchases, units sold, closing stock and stockout days by month.
### Task 8 — Benchmark Analysis
Classify products and suppliers as within or outside stock, defect and lead-time benchmarks.
### Task 9 — Inventory Dashboard
Build an operations dashboard with stock risk indicators.
### Task 10 — Inventory Recommendations
Recommend which products to reorder, which suppliers to review and where excess stock exists.

---

## 7. Recommended Pivot Charts

1. **Inventory Value by Warehouse** — Column Chart
2. **Units Sold by Product** — Bar Chart
3. **Stockout Days by Category** — Bar Chart
4. **Supplier Lead Time** — Column Chart
5. **Monthly Inventory Trend** — Line Chart
6. **Defect Rate by Supplier** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Inventory Value
- Units Sold
- Stockout Days
- Reorder Risk SKUs
- Defect Rate
- Average Lead Time
- Purchases
- Closing Stock

### Filters / Slicers

- Warehouse
- Category
- Product
- Supplier
- Month

### Dashboard Charts

- Inventory Value by Warehouse
- Stockout Days by Category
- Supplier Lead Time
- Monthly Inventory Trend

---

## 9. Final Business Questions

1. Which warehouse has the highest inventory value?
2. Which product sells the most?
3. Which warehouse has the most stockout days?
4. Which supplier has the highest defect rate?
5. Which SKUs are below reorder level?
6. Which category carries the most inventory value?
7. Which suppliers exceed the lead-time benchmark?
8. Where is capital tied up in excess stock?
9. What three inventory actions should management take?

---

## 10. Final Management Challenge

The operations manager can release budget for inventory improvements only if you identify the biggest sources of stockout and excess-stock risk.

---

## 11. Final Deliverable

Create an Excel workbook with:

1. **Raw Data**
2. **Analysis / Pivot Tables**
3. **KPI / Benchmark Analysis**
4. **Charts**
5. **Dashboard**
6. **Management Recommendations**

### Expected Workflow

```text
Raw Data
   ↓
Excel Table
   ↓
Pivot Tables
   ↓
Calculated KPIs
   ↓
Benchmark Comparison
   ↓
Pivot Charts
   ↓
Slicers / Timeline
   ↓
Dashboard
   ↓
Business Insights
   ↓
Management Decisions
```
