# Project 9: Digital Marketing Analytics

## 1. Business Scenario

A digital marketing team wants to evaluate social and online campaign performance across platforms, content types and campaigns.

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
| Date | Date of digital activity |
| Platform | Digital platform |
| Content_Type | Content type |
| Campaign | Campaign name |
| Impressions | Impressions |
| Reach | Unique users reached |
| Likes | Likes |
| Comments | Comments |
| Shares | Shares |
| Clicks | Clicks |
| Leads | Leads |
| Spend | Campaign spend |
| Conversions | Conversions |
| Revenue | Attributed revenue |
| Followers_Added | New followers |

---

## 3. Dataset

Save the following data as:

`09_digital_marketing_analytics.csv`

```csv
Date,Platform,Content_Type,Campaign,Impressions,Reach,Likes,Comments,Shares,Clicks,Leads,Spend,Conversions,Revenue,Followers_Added
2026-01-02,LinkedIn,Video,Campaign B,482961,238582,4182,104,143,18908,2421,40669,838,170371,789
2026-02-03,YouTube,Carousel,Campaign C,102042,90292,1122,131,63,1467,156,6075,21,9920,80
2026-03-04,Instagram,Short Video,Campaign D,490656,272700,26708,3198,2144,31577,3652,15515,481,22791,1627
2026-04-05,Facebook,Video,Campaign B,240425,119273,12233,1222,1561,3401,495,37631,122,184462,1834
2026-05-06,Google,Short Video,Campaign A,533220,409332,8324,693,392,18227,1824,47344,253,199791,192
2026-06-07,LinkedIn,Short Video,Campaign A,315617,202188,8667,430,232,17359,982,35928,271,99077,705
2026-01-08,Facebook,Article,Campaign A,465035,369503,4057,59,494,18901,3009,25315,530,124039,1038
2026-02-09,LinkedIn,Short Video,Campaign C,769265,545656,61328,7338,6210,7295,533,75300,53,135839,973
2026-03-10,LinkedIn,Short Video,Campaign D,894654,756786,68603,847,4741,53079,3645,10175,1175,46721,2309
2026-04-11,YouTube,Image,Campaign C,248994,170150,11876,541,960,17448,2975,77682,312,118900,654
2026-05-12,Instagram,Short Video,Campaign D,617915,360588,3634,291,251,11687,388,52720,118,220208,1333
2026-06-13,Instagram,Carousel,Campaign B,249092,164907,10674,754,1064,7272,877,19478,92,72289,293
2026-01-14,LinkedIn,Video,Campaign C,965923,401473,8742,271,210,51320,4722,69213,1312,290352,2437
2026-02-15,LinkedIn,Short Video,Campaign D,281444,197848,3520,395,165,11779,2057,15480,581,78094,268
2026-03-16,Instagram,Video,Campaign B,911957,533070,46871,4715,2557,7340,364,44833,27,257076,2147
2026-04-17,Google,Image,Campaign D,607487,360036,11248,925,1058,46207,5960,78156,1148,373688,2635
2026-05-18,Google,Image,Campaign C,786677,576336,61731,1750,2682,27625,3592,25732,1086,146180,1310
2026-06-19,LinkedIn,Article,Campaign D,482373,377260,21641,1944,2144,22785,1559,54160,469,208036,1060
2026-01-20,LinkedIn,Video,Campaign C,466379,186597,2577,106,57,7056,829,5860,117,34721,899
2026-02-21,Facebook,Carousel,Campaign C,630557,413415,30085,2192,970,24924,1386,23141,204,68543,2404
2026-03-22,Google,Video,Campaign C,900472,495395,36041,2616,1739,9716,955,68246,135,241845,2844
2026-04-23,Facebook,Short Video,Campaign A,89186,68262,5009,93,136,5602,524,61925,132,350816,513
2026-05-24,Instagram,Article,Campaign D,714678,563673,29352,1277,744,32514,2200,47838,624,217628,647
2026-06-25,Google,Article,Campaign C,839410,585543,38364,1320,2212,29021,1952,49062,181,170937,221
2026-01-26,Google,Short Video,Campaign B,139211,83424,4821,418,574,5717,373,68944,68,298582,823
2026-02-27,LinkedIn,Short Video,Campaign A,304085,132526,12648,576,1772,3563,529,60514,119,173788,1333
2026-03-01,Facebook,Image,Campaign B,857069,473452,56171,4369,8353,32710,2175,62732,153,353571,976
2026-04-02,LinkedIn,Article,Campaign D,844541,645434,12546,1146,647,43557,2515,42707,139,121616,475
2026-05-03,Instagram,Article,Campaign A,73853,41796,3820,127,347,4525,696,68311,193,321309,598
2026-06-04,LinkedIn,Video,Campaign A,317865,154215,6360,615,638,2854,420,6092,29,18675,1131
2026-01-05,Instagram,Carousel,Campaign B,356703,297385,24217,857,1682,27910,1652,46347,330,248443,2197
2026-02-06,Instagram,Image,Campaign C,574970,507926,36405,3217,916,42645,3776,48721,1191,150465,663
2026-03-07,LinkedIn,Carousel,Campaign B,422640,301179,10837,1274,922,27848,2945,55747,981,331902,2293
2026-04-08,LinkedIn,Short Video,Campaign C,408388,346553,28508,560,1986,31464,2806,59700,386,235809,1766
2026-05-09,Facebook,Short Video,Campaign B,520988,349643,11448,288,1034,33868,2147,45501,643,253254,1781
2026-06-10,YouTube,Image,Campaign D,382918,166150,11402,1016,500,26024,1376,8864,459,24196,1715
2026-01-11,Google,Image,Campaign B,831828,721098,78134,8802,4343,52765,2456,22241,311,29486,2526
2026-02-12,YouTube,Article,Campaign D,675329,348531,29838,1477,3266,27516,4940,66441,1705,286887,773
2026-03-13,Facebook,Article,Campaign D,194192,93579,3264,179,476,14449,2124,34170,313,165291,290
2026-04-14,Google,Short Video,Campaign A,771276,433802,26171,972,1900,6275,940,54856,207,169610,2362
2026-05-15,Instagram,Carousel,Campaign C,595940,270948,16327,1739,2189,13962,2038,10144,672,31035,2603
2026-06-16,YouTube,Article,Campaign A,510905,306042,13313,1345,1064,18742,3073,12149,859,44725,602
2026-01-17,YouTube,Short Video,Campaign B,807750,525303,15640,1163,2131,37140,4334,59206,878,199183,752
2026-02-18,LinkedIn,Video,Campaign D,975419,611920,22952,1975,3165,63145,3918,16952,428,77807,2617
2026-03-19,Facebook,Carousel,Campaign B,812182,646117,42826,4902,2964,27245,3963,27398,884,107245,2721
2026-04-20,Instagram,Short Video,Campaign C,237555,186380,2915,127,334,18308,1731,28684,206,158134,850
2026-05-21,YouTube,Article,Campaign A,62800,39521,4113,287,85,4471,377,33426,93,145919,1878
2026-06-22,LinkedIn,Video,Campaign B,680421,476329,17585,1234,1768,31854,2655,11411,321,21813,2695
2026-01-23,Google,Short Video,Campaign B,945304,393450,28954,2210,1825,10944,551,59651,72,117775,1184
2026-02-24,LinkedIn,Article,Campaign B,527456,408602,20275,282,2431,15407,2014,13869,537,72782,285
2026-03-25,Google,Video,Campaign D,177950,132983,5344,363,471,10176,1558,12626,132,49778,2596
2026-04-26,LinkedIn,Carousel,Campaign D,809246,602343,67900,8045,3893,40999,3821,39034,1267,154601,2572
2026-05-27,Instagram,Carousel,Campaign D,594951,454894,29455,2912,3972,13359,994,30369,49,53673,1924
2026-06-01,LinkedIn,Short Video,Campaign C,484153,204673,9918,978,472,25682,3596,41913,700,209269,1280
2026-01-02,YouTube,Article,Campaign A,854291,344335,29420,1398,3358,43739,1550,28020,176,78076,1404
2026-02-03,LinkedIn,Short Video,Campaign C,727015,340153,9215,559,1220,52486,5362,59257,1788,87043,2154
2026-03-04,LinkedIn,Article,Campaign B,632145,422236,13895,1186,1722,45262,4253,13678,517,34827,147
2026-04-05,Facebook,Image,Campaign D,648717,455947,13957,318,1698,18242,1835,9145,369,29141,2055
2026-05-06,Google,Carousel,Campaign B,919749,805114,27193,1176,940,58745,5073,17137,1161,62186,1996
2026-06-07,Facebook,Video,Campaign D,406637,350447,31739,2145,3834,6403,1084,17878,318,79525,563
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| Engagement Rate | 5% or higher |
| CTR | 2% or higher |
| Lead Conversion Rate | 10% or higher |
| CPL | ₹1,200 or lower |
| ROAS | 3× or higher |
| Follower Growth | Positive monthly growth |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **Engagement Rate**: `(Likes + Comments + Shares) / Reach × 100`
- **CTR**: `Clicks / Impressions × 100`
- **CPL**: `Spend / Leads`
- **Lead Conversion Rate**: `Conversions / Leads × 100`
- **ROAS**: `Revenue / Spend`
- **Follower Growth**: `Sum Followers_Added`

---

## 6. Assignment Tasks

### Task 1 — Platform Performance
Compare platforms by reach, engagement, clicks, leads, conversions, spend and revenue.
### Task 2 — Content Performance
Identify which content types produce the strongest engagement and conversion.
### Task 3 — Campaign Performance
Compare campaigns by reach, leads, conversions, revenue and ROAS.
### Task 4 — Engagement Analysis
Calculate engagement rate by platform and content type.
### Task 5 — Traffic Analysis
Calculate CTR and compare platforms.
### Task 6 — Lead Generation
Calculate CPL and lead conversion rate by campaign.
### Task 7 — Monthly Trend
Analyze reach, engagement, leads, revenue and follower growth by month.
### Task 8 — Benchmark Analysis
Classify platform/content/campaign combinations against engagement, CTR, CPL and ROAS benchmarks.
### Task 9 — Digital Marketing Dashboard
Create a dashboard with platform, content type and campaign slicers.
### Task 10 — Content Strategy
Recommend which platforms and content types deserve more investment.

---

## 7. Recommended Pivot Charts

1. **Reach by Platform** — Column Chart
2. **Engagement Rate by Content** — Bar Chart
3. **ROAS by Campaign** — Bar Chart
4. **Monthly Lead Trend** — Line Chart
5. **CTR by Platform** — Column Chart
6. **Revenue by Campaign** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Reach
- Impressions
- Engagement Rate
- CTR
- Leads
- CPL
- Conversions
- ROAS

### Filters / Slicers

- Platform
- Content_Type
- Campaign
- Month

### Dashboard Charts

- Reach by Platform
- Engagement by Content
- ROAS by Campaign
- Monthly Lead Trend

---

## 9. Final Business Questions

1. Which platform reaches the most people?
2. Which content type has the highest engagement?
3. Which campaign has the best ROAS?
4. Which platform has the best CTR?
5. Which campaign has the lowest CPL?
6. Which platforms exceed the engagement benchmark?
7. Which content type converts best?
8. Where should the next content budget be allocated?
9. What three content strategy changes would you recommend?

---

## 10. Final Management Challenge

The marketing head wants a content and platform strategy for the next quarter. Use the data to identify which combinations create attention, leads and revenue—not just likes.

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
