# Project 3: Marketing Campaign Analytics

## 1. Business Scenario

A marketing team runs campaigns across several platforms for multiple clients. Management wants to understand campaign efficiency, lead generation, conversion performance and return on advertising spend.

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
| Campaign_ID | Campaign identifier |
| Month | Campaign month |
| Client | Client account |
| Platform | Marketing platform |
| Campaign_Type | Campaign type |
| Audience | Audience segment |
| Ad_Spend | Advertising spend |
| Impressions | Ad impressions |
| Clicks | Ad clicks |
| Leads | Leads generated |
| Conversions | Conversions |
| Revenue | Revenue attributed to campaign |
| Engagement_Rate | Engagement rate % |
| Campaign_Rating | Internal campaign rating out of 5 |

---

## 3. Dataset

Save the following data as:

`03_marketing_campaign_analytics.csv`

```csv
Campaign_ID,Month,Client,Platform,Campaign_Type,Audience,Ad_Spend,Impressions,Clicks,Leads,Conversions,Revenue,Engagement_Rate,Campaign_Rating
CMP001,2026-01,Client D,Email,Lead Generation,Students,37275,181164,6869,693,184,104186,2.63,3.3
CMP002,2026-02,Client A,Email,Remarketing,Enterprise,82422,1090101,52903,9995,2930,159586,4.77,4.8
CMP003,2026-03,Client D,Google Ads,Lead Generation,SMB,104323,215327,2072,307,66,334365,2.2,4.4
CMP004,2026-04,Client D,Email,Remarketing,Enterprise,99730,461078,6609,456,92,398647,5.3,4.4
CMP005,2026-05,Client B,YouTube,Product Launch,Professionals,86263,1419672,63485,3528,410,423652,5.73,4.5
CMP006,2026-06,Client C,LinkedIn,Brand Awareness,Enterprise,74239,860791,58528,9185,2092,234889,2.12,3.9
CMP007,2026-01,Client A,Email,Remarketing,Students,28799,341312,4503,230,66,54322,6.3,4.6
CMP008,2026-02,Client B,Meta Ads,Product Launch,Professionals,73845,891548,59892,2638,425,288116,3.79,4.2
CMP009,2026-03,Client A,Email,Remarketing,Students,131054,376950,13356,1905,212,596351,5.23,4.6
CMP010,2026-04,Client D,Google Ads,Brand Awareness,Students,43647,723089,49667,6552,2214,124799,1.54,4.7
CMP011,2026-05,Client C,Email,Lead Generation,Students,32026,1262502,34509,4116,1064,106152,2.52,3.7
CMP012,2026-06,Client D,YouTube,Remarketing,Professionals,40392,480112,5661,859,83,104551,5.8,4.0
CMP013,2026-01,Client C,Google Ads,Brand Awareness,Enterprise,118951,1224468,21040,2044,542,231188,5.91,4.2
CMP014,2026-02,Client C,LinkedIn,Remarketing,Students,149033,1406875,14214,457,74,403235,2.87,3.4
CMP015,2026-03,Client C,Google Ads,Product Launch,Students,21013,1193092,62411,4750,501,63476,6.07,4.1
CMP016,2026-04,Client D,LinkedIn,Lead Generation,Enterprise,77176,189303,8532,414,130,212407,4.29,3.9
CMP017,2026-05,Client A,Meta Ads,Product Launch,Enterprise,22733,831088,15418,2993,620,109757,7.48,3.3
CMP018,2026-06,Client A,Email,Brand Awareness,SMB,88676,314934,14542,1706,432,211606,6.56,3.3
CMP019,2026-01,Client A,Meta Ads,Product Launch,Enterprise,66019,459728,17782,954,121,166623,2.63,3.5
CMP020,2026-02,Client C,Meta Ads,Product Launch,Students,118886,1332238,106259,17896,5518,484099,7.91,3.7
CMP021,2026-03,Client D,YouTube,Lead Generation,Students,81462,1077377,45077,7875,1518,314905,3.79,3.3
CMP022,2026-04,Client D,YouTube,Lead Generation,Enterprise,68331,752044,8788,1583,521,369634,2.09,4.2
CMP023,2026-05,Client D,Google Ads,Remarketing,Students,139150,1348850,92181,5849,950,545471,4.76,4.8
CMP024,2026-06,Client B,LinkedIn,Remarketing,SMB,86132,511882,5124,406,110,280017,4.36,4.1
CMP025,2026-01,Client D,LinkedIn,Remarketing,Professionals,70779,1007251,49386,2338,762,289431,1.93,3.4
CMP026,2026-02,Client D,Meta Ads,Lead Generation,SMB,63694,320922,20699,3338,310,329105,3.52,4.3
CMP027,2026-03,Client A,YouTube,Remarketing,Students,93259,939953,47753,8093,927,389866,6.89,4.5
CMP028,2026-04,Client B,Meta Ads,Lead Generation,SMB,67526,797739,15801,1351,241,357257,4.66,3.6
CMP029,2026-05,Client B,Email,Product Launch,Professionals,130680,362107,18445,2763,894,657938,1.75,3.8
CMP030,2026-06,Client D,Email,Remarketing,Enterprise,41266,529261,13494,2196,153,129716,5.9,3.6
CMP031,2026-01,Client D,YouTube,Remarketing,Enterprise,50671,1269902,37697,3665,1143,259227,2.76,4.4
CMP032,2026-02,Client D,LinkedIn,Lead Generation,Students,85916,1256163,61154,4489,632,404237,2.4,3.6
CMP033,2026-03,Client B,YouTube,Remarketing,Students,57363,325898,6882,764,153,293768,2.46,3.9
CMP034,2026-04,Client A,LinkedIn,Lead Generation,SMB,74381,261687,14299,2484,506,181721,7.96,3.8
CMP035,2026-05,Client D,YouTube,Lead Generation,Students,123727,456287,11298,416,56,639617,4.57,4.6
CMP036,2026-06,Client C,Meta Ads,Remarketing,Students,22490,686711,17566,1138,336,118317,5.46,3.9
CMP037,2026-01,Client A,Email,Brand Awareness,Professionals,26258,650043,30763,6024,1237,45983,6.94,4.0
CMP038,2026-02,Client A,Email,Remarketing,Students,58177,1050179,5455,792,129,143246,4.21,4.3
CMP039,2026-03,Client D,LinkedIn,Remarketing,Students,144964,1253226,77579,10639,2610,538774,4.04,4.0
CMP040,2026-04,Client C,Meta Ads,Lead Generation,SMB,66805,291682,12756,1369,443,275798,2.17,4.2
CMP041,2026-05,Client B,Google Ads,Product Launch,Students,91567,859985,57613,4596,1180,496593,4.61,3.5
CMP042,2026-06,Client D,Email,Product Launch,SMB,58462,572766,5733,981,151,294833,3.55,3.7
CMP043,2026-01,Client C,YouTube,Product Launch,Enterprise,24799,550772,21503,2107,153,123082,3.66,3.4
CMP044,2026-02,Client C,Google Ads,Product Launch,Students,137261,960852,49242,4537,1242,585867,3.89,4.6
CMP045,2026-03,Client C,YouTube,Product Launch,Professionals,76440,1413436,30719,5389,870,212873,2.02,4.3
CMP046,2026-04,Client D,LinkedIn,Lead Generation,Students,110408,1080943,51481,8869,616,486596,7.43,4.2
CMP047,2026-05,Client B,Email,Product Launch,Students,107973,1486960,60676,7772,2489,507946,5.92,4.8
CMP048,2026-06,Client B,YouTube,Remarketing,SMB,36545,290998,9187,1596,266,107756,7.67,3.3
CMP049,2026-01,Client A,Google Ads,Brand Awareness,Enterprise,78188,311240,20362,1173,329,232046,3.54,3.7
CMP050,2026-02,Client C,YouTube,Brand Awareness,Students,87861,961571,20242,1679,479,223268,4.4,4.9
CMP051,2026-03,Client C,LinkedIn,Lead Generation,SMB,37790,305298,16338,1197,286,207431,6.77,4.8
CMP052,2026-04,Client B,Meta Ads,Brand Awareness,Enterprise,136828,779054,59689,4370,1524,300524,3.85,3.6
CMP053,2026-05,Client D,YouTube,Product Launch,Enterprise,23445,906854,52887,9243,2721,47337,7.25,3.3
CMP054,2026-06,Client C,Meta Ads,Brand Awareness,Professionals,127916,1355653,16444,1006,212,520535,4.42,4.4
CMP055,2026-01,Client B,LinkedIn,Remarketing,Students,76704,1204581,13285,906,310,162003,2.57,3.7
CMP056,2026-02,Client B,Email,Brand Awareness,Professionals,52847,561674,44427,5844,854,105729,3.47,4.1
CMP057,2026-03,Client C,Meta Ads,Product Launch,Students,106341,1459627,101752,14115,1042,510537,1.68,3.3
CMP058,2026-04,Client C,YouTube,Lead Generation,Students,85278,1465258,78835,7110,1592,292655,6.73,4.4
CMP059,2026-05,Client C,LinkedIn,Product Launch,Professionals,40719,1071919,59835,9728,2388,94308,5.44,3.7
CMP060,2026-06,Client B,Meta Ads,Lead Generation,Students,119701,927079,72134,11366,1002,332345,4.53,3.7
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| CTR | 2.5% or higher |
| Conversion Rate | 10% or higher |
| CPL | ₹1,500 or lower |
| ROAS | 3.0 or higher |
| Campaign Rating | 4.0 or higher |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **CTR**: `Clicks / Impressions × 100`
- **CPC**: `Ad Spend / Clicks`
- **CPL**: `Ad Spend / Leads`
- **Conversion Rate**: `Conversions / Leads × 100`
- **ROAS**: `Revenue / Ad Spend`

---

## 6. Assignment Tasks

### Task 1 — Platform Performance
Create a Pivot Table by Platform showing Spend, Impressions, Clicks, Leads, Conversions and Revenue.
### Task 2 — Campaign Type Analysis
Compare campaign types using Spend, Leads, Conversion Rate, Revenue and ROAS.
### Task 3 — Client Performance
Compare clients by spend, revenue, leads, conversions and ROAS.
### Task 4 — Audience Analysis
Determine which audience segment provides the best conversion and revenue performance.
### Task 5 — Marketing Funnel
Create a Pivot Table by Platform with Impressions → Clicks → Leads → Conversions.
### Task 6 — Monthly Campaign Trend
Group Month and analyze Spend, Revenue, Leads, Conversions and ROAS.
### Task 7 — Benchmark Gap Analysis
Calculate CTR, CPL, Conversion Rate and ROAS and classify each campaign as Above/Below Benchmark.
### Task 8 — Budget Efficiency
Identify campaigns spending heavily but generating weak revenue or conversions.
### Task 9 — Marketing Dashboard
Create KPI cards, slicers for Platform, Client, Campaign Type and Audience, plus a month timeline.
### Task 10 — Recommendations
Recommend which platforms and campaign types should receive more or less budget.

---

## 7. Recommended Pivot Charts

1. **Spend vs Revenue by Platform** — Combo/Column Chart
2. **ROAS by Platform** — Bar Chart
3. **Conversions by Campaign Type** — Column Chart
4. **Monthly Revenue Trend** — Line Chart
5. **Marketing Funnel** — Funnel-style chart or staged columns
6. **CPL by Client** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Ad Spend
- Revenue
- Leads
- Conversions
- CTR
- CPL
- Conversion Rate
- ROAS

### Filters / Slicers

- Platform
- Client
- Campaign_Type
- Audience

### Dashboard Charts

- Revenue by Platform
- ROAS by Platform
- Conversions by Campaign Type
- Monthly Revenue Trend

---

## 9. Final Business Questions

1. Which platform generates the highest revenue?
2. Which platform has the best ROAS?
3. Which campaign type has the highest conversion rate?
4. Which client has the highest marketing ROI?
5. Which audience is most valuable?
6. Which campaigns are below the CPL benchmark?
7. Which campaigns exceed the ROAS benchmark?
8. Where is budget being wasted?
9. What three budget allocation changes would you recommend?

---

## 10. Final Management Challenge

The marketing director has a fixed budget for the next quarter. Use your analysis to recommend the platforms, campaign types and audiences that deserve more budget.

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
