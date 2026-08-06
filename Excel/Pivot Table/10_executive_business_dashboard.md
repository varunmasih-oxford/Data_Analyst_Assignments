# Project 10: Executive Business Dashboard

## 1. Business Scenario

Senior management wants a single executive-level view of business performance covering revenue, profit, customers, marketing, workforce and customer service. The analyst must consolidate operational indicators into a management dashboard.

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
| Month | Reporting month |
| Region | Business region |
| Department | Business department |
| Revenue | Revenue |
| Cost | Operating cost |
| Profit | Profit |
| Orders | Orders |
| Customers | Customers |
| New_Customers | New customers |
| Customer_Rating | Average customer rating |
| Employee_Count | Employees |
| Attrition_Rate | Employee attrition rate % |
| Marketing_Spend | Marketing spend |
| Leads | Leads |
| Conversions | Conversions |
| Tickets | Support tickets |
| SLA_Compliance | SLA compliance % |

---

## 3. Dataset

Save the following data as:

`10_executive_business_dashboard.csv`

```csv
Month,Region,Department,Revenue,Cost,Profit,Orders,Customers,New_Customers,Customer_Rating,Employee_Count,Attrition_Rate,Marketing_Spend,Leads,Conversions,Tickets,SLA_Compliance
2026-01,North,HR,4051325,3095630,955695,1269,387,42,4.1,36,10.6,361577,913,361,1056,97.1
2026-02,North,Operations,3421278,1904776,1516502,1753,789,367,4.8,107,5.2,200243,2466,565,753,95.1
2026-03,East,HR,2052593,1225908,826685,434,181,358,4.4,51,5.3,233667,4700,346,655,84.4
2026-04,North,Sales,2853741,1716189,1137552,837,1405,496,4.1,138,3.6,65200,4056,711,203,83.8
2026-05,North,Support,4377453,2922278,1455175,1643,1370,496,4.4,139,9.8,213808,2922,857,505,94.1
2026-06,South,HR,1905578,1101185,804393,1843,1580,279,3.8,104,10.5,422357,4012,501,574,98.1
2026-01,North,Operations,2964703,2442495,522208,1002,525,398,4.8,109,11.7,220268,3913,519,161,83.1
2026-02,North,Operations,4815224,3314667,1500557,549,728,433,4.1,172,4.4,103966,3523,857,319,87.5
2026-03,West,Support,4666937,3127990,1538947,1046,638,357,4.0,65,13.7,251230,741,368,526,95.8
2026-04,West,Marketing,3670588,2618443,1052145,683,504,379,4.5,171,12.2,109938,3992,353,1236,83.7
2026-05,North,Marketing,3383990,2831604,552386,342,1375,95,4.5,177,11.5,248658,2882,526,1420,93.2
2026-06,West,Marketing,1965318,1604050,361268,1746,1452,454,3.7,62,10.3,287489,4552,318,898,92.5
2026-01,West,Marketing,2525215,1905161,620054,848,763,331,4.7,102,13.1,277922,3020,111,1293,82.1
2026-02,West,IT,3267799,1858472,1409327,1324,258,40,4.5,116,4.2,197958,455,260,984,93.9
2026-03,South,Operations,3468645,2648421,820224,1031,931,262,4.4,69,8.2,148685,4750,413,837,96.3
2026-04,West,IT,1853182,1093902,759280,346,1477,48,3.9,149,10.2,121185,893,160,1415,95.7
2026-05,West,IT,4371065,3221363,1149702,1130,1193,257,4.4,140,7.2,168353,1722,454,1338,82.1
2026-06,West,IT,2786002,2127499,658503,751,991,319,4.4,33,13.8,347874,4158,741,854,83.9
2026-01,North,IT,1471618,872119,599499,1697,1228,479,4.9,96,8.1,91017,4487,644,281,86.2
2026-02,East,Operations,3421437,2511032,910405,903,1245,438,3.7,141,8.6,296012,4901,771,778,89.2
2026-03,East,IT,2205160,1236208,968952,1423,772,412,4.6,91,3.7,298072,4936,193,1273,82.9
2026-04,North,HR,1028992,654484,374508,368,409,298,3.8,96,5.8,372855,2501,301,626,82.2
2026-05,North,Operations,2264767,1863992,400775,1713,459,377,4.2,69,5.9,417407,2134,516,470,95.6
2026-06,East,Sales,1508010,1267035,240975,1419,465,468,4.3,130,11.5,174752,3805,763,1405,84.8
2026-01,West,Support,3017910,2343845,674065,437,257,125,4.3,146,6.3,441197,4562,259,877,93.6
2026-02,East,Support,3003059,1782450,1220609,1982,1040,46,4.0,139,7.2,215511,4543,719,184,83.7
2026-03,South,HR,3086655,2007838,1078817,746,351,170,4.5,125,8.1,404047,2180,771,1476,92.0
2026-04,West,Operations,3630371,2734814,895557,568,791,320,3.7,27,12.1,56271,3568,120,1175,83.8
2026-05,North,Sales,2640597,2026856,613741,715,545,57,3.7,48,3.6,361499,1976,633,1406,84.1
2026-06,North,IT,1889741,1252496,637245,1764,1476,329,4.7,72,12.9,414722,1709,279,703,89.9
2026-01,East,Sales,4603761,3806429,797332,766,1024,394,4.8,107,5.8,459328,806,303,227,88.5
2026-02,West,Marketing,2966262,2481817,484445,742,514,265,3.8,76,9.7,143555,4230,131,394,91.2
2026-03,North,Sales,1691287,1393253,298034,1665,680,92,3.7,43,9.3,181384,3852,39,1119,84.5
2026-04,North,HR,4075615,2567356,1508259,1633,825,240,4.4,156,10.8,454221,4219,509,993,88.9
2026-05,North,Operations,2694540,1484670,1209870,1611,1137,102,4.4,116,6.7,208769,3481,76,1394,98.9
2026-06,East,Support,3652653,2097123,1555530,1141,743,371,3.9,166,3.4,251412,1764,326,898,97.2
2026-01,East,Support,1511878,1233033,278845,1096,538,111,3.7,31,10.9,360874,2153,520,896,83.1
2026-02,South,IT,4569062,3837885,731177,233,225,213,3.8,35,7.5,160980,4485,489,1488,96.8
2026-03,South,IT,2754425,2279134,475291,275,439,290,4.5,145,13.0,374205,575,268,1428,84.2
2026-04,South,Sales,1219078,1001349,217729,1880,349,273,4.4,176,3.7,478589,1071,136,1118,92.1
2026-05,East,Sales,2499877,1694575,805302,1861,1539,245,4.1,172,9.0,218605,1946,802,193,92.1
2026-06,West,Marketing,1812886,1146048,666838,1751,1000,126,4.5,166,4.8,177739,4967,61,373,83.7
2026-01,South,Marketing,931116,757824,173292,365,163,43,3.9,47,10.8,361285,2524,446,1074,93.8
2026-02,East,Operations,3072891,2172306,900585,1043,639,129,4.4,34,9.6,426018,4295,646,280,92.7
2026-03,South,Operations,4313030,2378079,1934951,682,543,100,4.9,49,9.8,449050,4621,539,549,89.9
2026-04,South,Support,1245175,757210,487965,1831,455,390,4.7,146,8.5,133760,553,75,1420,88.2
2026-05,North,Sales,2908743,1891521,1017222,1848,1078,62,3.8,38,13.2,142215,1494,824,159,90.2
2026-06,West,Marketing,2773838,2125927,647911,1413,1337,206,4.2,108,5.5,107741,2871,253,300,86.0
2026-01,West,IT,3950193,3228925,721268,350,1114,339,4.3,136,4.6,369518,3927,202,893,88.3
2026-02,South,Operations,2428689,1796273,632416,752,564,211,3.9,170,3.7,121566,1110,892,1053,89.8
2026-03,West,Marketing,2644265,2157515,486750,1436,471,444,4.7,68,9.4,339803,2081,108,943,96.6
2026-04,North,Support,4771913,3822763,949150,771,179,413,4.2,88,5.7,277671,4946,247,1311,98.1
2026-05,North,IT,1170979,658110,512869,1163,1182,57,4.2,125,8.3,468391,1002,483,1114,86.1
2026-06,North,Support,4210959,3516067,694892,471,884,191,4.0,48,3.2,400767,2697,185,1040,96.6
2026-01,East,HR,4690306,3665711,1024595,1990,1590,247,3.9,119,9.9,419047,211,662,244,88.5
2026-02,North,HR,1074426,686533,387893,1741,702,397,4.8,163,9.3,158604,863,655,787,94.5
2026-03,South,Marketing,3853373,3145868,707505,427,934,227,4.3,35,7.0,141890,4777,741,237,91.5
2026-04,East,HR,3609593,2243686,1365907,432,1479,284,4.6,173,12.6,418492,1918,791,561,87.4
2026-05,East,Support,4347786,2752772,1595014,329,913,216,4.2,153,8.8,114335,4051,746,1189,93.5
2026-06,East,Sales,3888231,3071590,816641,1619,284,136,4.8,142,4.0,254830,1664,315,257,83.9
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| Profit Margin | 20% or higher |
| Customer Rating | 4.3 or higher |
| Attrition Rate | 10% or lower |
| Marketing Conversion Rate | 10% or higher |
| SLA Compliance | 90% or higher |
| Revenue Growth | Positive month-over-month |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **Profit Margin**: `Profit / Revenue × 100`
- **Average Order Value**: `Revenue / Orders`
- **Customer Growth**: `New Customers / Customers × 100`
- **Marketing Conversion Rate**: `Conversions / Leads × 100`
- **Marketing ROAS**: `Revenue / Marketing Spend`
- **SLA Compliance**: `Average SLA Compliance`
- **Attrition Rate**: `Average Attrition Rate`

---

## 6. Assignment Tasks

### Task 1 — Executive KPI Summary
Create a Pivot Table by Month with Revenue, Cost, Profit, Orders, Customers, Leads, Conversions and SLA Compliance.
### Task 2 — Regional Performance
Compare regions by Revenue, Profit, Profit Margin, Customers and Customer Rating.
### Task 3 — Department Performance
Compare departments by cost, profit contribution, employee count and relevant operational KPIs.
### Task 4 — Revenue & Profit Trend
Create monthly trends for Revenue, Cost and Profit.
### Task 5 — Customer Growth
Analyze customers and new customers by region and month.
### Task 6 — Marketing Efficiency
Calculate lead conversion rate and compare marketing spend with conversions.
### Task 7 — Workforce Risk
Analyze employee count and attrition rate by department and region.
### Task 8 — Customer Service
Compare ticket volume and SLA compliance across departments/regions.
### Task 9 — Benchmark Scorecard
Create an executive scorecard showing Actual, Benchmark, Gap and Status for every major KPI.
### Task 10 — Executive Dashboard
Create a one-page dashboard designed for senior management with minimal clutter and strong KPI hierarchy.

---

## 7. Recommended Pivot Charts

1. **Revenue vs Profit Trend** — Line/Column Chart
2. **Profit by Region** — Bar Chart
3. **Revenue by Department** — Column Chart
4. **Customer Growth Trend** — Line Chart
5. **Marketing Conversion Rate** — Column Chart
6. **SLA Compliance** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Revenue
- Profit
- Profit Margin
- Customers
- New Customers
- Marketing Conversion Rate
- Attrition Rate
- SLA Compliance

### Filters / Slicers

- Month
- Region
- Department

### Dashboard Charts

- Revenue vs Profit Trend
- Profit by Region
- Revenue by Department
- Customer Growth Trend
- Marketing Conversion Rate
- SLA Compliance

---

## 9. Final Business Questions

1. Which region produces the most profit?
2. Which department has the strongest contribution?
3. Is the company profit margin above benchmark?
4. Which region has the strongest customer rating?
5. Which month has the best revenue and profit?
6. Is marketing conversion above benchmark?
7. Which region has the highest attrition risk?
8. Which area has the weakest SLA performance?
9. Which three KPIs should executives monitor most closely?
10. What three strategic actions should senior management take?

---

## 10. Final Management Challenge

The CEO has five minutes to review your dashboard. Identify the strongest and weakest parts of the business, quantify the gaps against benchmarks, and provide three strategic actions that management should take next.

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
