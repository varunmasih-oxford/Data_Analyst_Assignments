# Project 4: Customer Support Analytics

## 1. Business Scenario

A customer support department wants to improve service quality, reduce resolution time and ensure that support agents meet SLA expectations.

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
| Ticket_ID | Support ticket identifier |
| Date | Ticket date |
| Channel | Support channel |
| Customer_Type | New or Existing |
| Issue_Category | Issue category |
| Priority | Low/Medium/High/Critical |
| Agent | Support agent |
| First_Response_Min | Minutes to first response |
| Resolution_Hours | Hours to resolution |
| SLA_Met | SLA met Yes/No |
| CSAT | Customer satisfaction out of 5 |
| Escalated | Escalated Yes/No |
| Reopened | Reopened Yes/No |

---

## 3. Dataset

Save the following data as:

`04_customer_support_analytics.csv`

```csv
Ticket_ID,Date,Channel,Customer_Type,Issue_Category,Priority,Agent,First_Response_Min,Resolution_Hours,SLA_Met,CSAT,Escalated,Reopened
TKT001,2026-01-02,Phone,Existing,Refund,High,Agent C,103,31.2,No,4.0,No,No
TKT002,2026-02-03,Web,Existing,Delivery,Medium,Agent A,45,18.4,Yes,4.1,No,No
TKT003,2026-03-04,Phone,Existing,Billing,Low,Agent A,105,18.7,No,4.9,No,No
TKT004,2026-04-05,Chat,New,Billing,High,Agent D,131,21.9,No,4.7,No,No
TKT005,2026-05-06,Chat,New,Delivery,Medium,Agent A,72,26.5,No,4.6,No,No
TKT006,2026-06-07,Chat,New,Technical,Medium,Agent A,97,20.4,No,3.3,No,No
TKT007,2026-01-08,Phone,New,Refund,Critical,Agent E,26,14.5,Yes,3.8,No,No
TKT008,2026-02-09,Web,New,Refund,Critical,Agent E,35,1.7,Yes,3.3,No,No
TKT009,2026-03-10,Web,Existing,Refund,Medium,Agent C,88,33.6,No,3.8,No,No
TKT010,2026-04-11,Chat,New,Delivery,Critical,Agent E,48,10.6,Yes,4.1,Yes,No
TKT011,2026-05-12,Phone,New,Refund,High,Agent D,166,1.9,No,4.1,No,No
TKT012,2026-06-13,Web,New,Product,Medium,Agent B,139,23.0,No,4.3,No,No
TKT013,2026-01-14,Chat,Existing,Technical,Low,Agent D,151,34.2,No,3.4,No,Yes
TKT014,2026-02-15,Web,New,Product,Medium,Agent B,110,18.6,No,4.3,No,No
TKT015,2026-03-16,Web,Existing,Technical,Medium,Agent D,148,12.4,No,4.4,No,No
TKT016,2026-04-17,Chat,Existing,Technical,High,Agent B,144,13.4,No,4.6,No,No
TKT017,2026-05-18,Chat,New,Product,High,Agent D,147,11.4,No,4.9,No,No
TKT018,2026-06-19,Chat,Existing,Billing,High,Agent E,127,13.2,No,4.9,No,No
TKT019,2026-01-20,Phone,Existing,Billing,Critical,Agent C,60,17.7,Yes,4.7,No,No
TKT020,2026-02-21,Web,New,Technical,Low,Agent E,93,33.3,No,4.4,No,No
TKT021,2026-03-22,Phone,New,Product,High,Agent E,148,25.4,No,3.4,No,No
TKT022,2026-04-23,Web,New,Product,Medium,Agent B,168,9.1,No,3.4,No,Yes
TKT023,2026-05-24,Web,Existing,Product,Low,Agent B,145,35.2,No,3.5,No,No
TKT024,2026-06-25,Phone,New,Technical,High,Agent D,87,11.0,No,3.3,No,No
TKT025,2026-01-26,Web,New,Product,Medium,Agent C,14,35.9,No,3.9,No,No
TKT026,2026-02-27,Chat,Existing,Delivery,Low,Agent E,7,11.4,Yes,4.3,No,No
TKT027,2026-03-01,Phone,New,Account,Critical,Agent B,59,17.0,Yes,4.7,No,No
TKT028,2026-04-02,Phone,New,Refund,Critical,Agent D,44,5.4,Yes,3.5,No,No
TKT029,2026-05-03,Phone,Existing,Account,Critical,Agent B,35,6.6,Yes,3.9,Yes,No
TKT030,2026-06-04,Chat,Existing,Account,Low,Agent E,71,14.4,No,4.0,No,No
TKT031,2026-01-05,Email,New,Delivery,Low,Agent C,71,23.9,No,4.4,No,No
TKT032,2026-02-06,Chat,New,Product,Medium,Agent C,108,25.0,No,4.9,No,No
TKT033,2026-03-07,Web,Existing,Delivery,High,Agent E,162,8.7,No,4.9,No,No
TKT034,2026-04-08,Phone,New,Refund,Critical,Agent D,51,10.1,Yes,4.4,Yes,No
TKT035,2026-05-09,Phone,New,Technical,High,Agent C,24,33.1,No,3.4,No,No
TKT036,2026-06-10,Web,New,Delivery,Critical,Agent B,10,12.6,Yes,4.5,No,No
TKT037,2026-01-11,Chat,New,Delivery,Critical,Agent C,32,10.6,Yes,4.2,No,No
TKT038,2026-02-12,Email,New,Billing,Low,Agent D,60,21.2,Yes,3.3,No,Yes
TKT039,2026-03-13,Web,Existing,Delivery,Low,Agent D,78,15.3,No,4.6,No,No
TKT040,2026-04-14,Phone,Existing,Billing,Critical,Agent B,27,2.4,Yes,4.9,No,No
TKT041,2026-05-15,Email,Existing,Delivery,Critical,Agent E,36,3.2,Yes,5.0,No,No
TKT042,2026-06-16,Phone,New,Billing,Critical,Agent D,37,7.4,Yes,3.6,No,Yes
TKT043,2026-01-17,Email,New,Product,Low,Agent A,66,8.2,No,3.4,No,Yes
TKT044,2026-02-18,Chat,New,Product,Critical,Agent E,31,5.0,Yes,3.6,No,Yes
TKT045,2026-03-19,Chat,New,Product,High,Agent E,152,21.9,No,4.4,Yes,No
TKT046,2026-04-20,Phone,Existing,Refund,Medium,Agent D,110,11.5,No,3.3,No,No
TKT047,2026-05-21,Chat,Existing,Delivery,Low,Agent B,93,34.0,No,4.4,No,No
TKT048,2026-06-22,Phone,Existing,Product,High,Agent B,101,7.4,No,4.2,Yes,No
TKT049,2026-01-23,Phone,Existing,Technical,Critical,Agent C,6,10.6,Yes,4.9,No,No
TKT050,2026-02-24,Chat,New,Refund,Medium,Agent B,89,23.6,No,4.9,No,No
TKT051,2026-03-25,Email,New,Technical,Low,Agent E,73,14.2,No,4.3,No,No
TKT052,2026-04-26,Chat,New,Technical,Medium,Agent B,127,8.3,No,4.8,No,No
TKT053,2026-05-27,Phone,Existing,Technical,Low,Agent E,127,33.0,No,4.5,No,No
TKT054,2026-06-01,Chat,Existing,Refund,High,Agent D,77,14.3,No,4.2,No,No
TKT055,2026-01-02,Chat,New,Account,Critical,Agent C,9,14.6,Yes,4.5,No,No
TKT056,2026-02-03,Web,Existing,Technical,Critical,Agent B,5,10.6,Yes,3.6,Yes,Yes
TKT057,2026-03-04,Chat,Existing,Delivery,High,Agent D,63,14.3,No,4.7,No,No
TKT058,2026-04-05,Web,New,Refund,Critical,Agent A,13,13.5,Yes,3.8,Yes,No
TKT059,2026-05-06,Email,Existing,Technical,Low,Agent B,24,34.1,No,4.4,No,No
TKT060,2026-06-07,Chat,New,Refund,Low,Agent E,43,1.3,Yes,4.1,No,No
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| First Response Time | 60 minutes or less |
| Resolution Time | 24 hours or less |
| SLA Compliance | 90% or higher |
| CSAT | 4.2 or higher |
| Escalation Rate | 10% or lower |
| Reopen Rate | 8% or lower |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **SLA Compliance**: `SLA Met Yes tickets / Total Tickets × 100`
- **Escalation Rate**: `Escalated Yes / Total Tickets × 100`
- **Reopen Rate**: `Reopened Yes / Total Tickets × 100`
- **Average Response Time**: `Average First_Response_Min`
- **Average Resolution Time**: `Average Resolution_Hours`
- **Average CSAT**: `Average CSAT`

---

## 6. Assignment Tasks

### Task 1 — Agent Performance
Create a Pivot Table by Agent with ticket count, average response time, average resolution time, SLA compliance, CSAT and escalation rate.
### Task 2 — Issue Analysis
Compare Issue Category by ticket volume, resolution time, CSAT and reopen rate.
### Task 3 — Channel Analysis
Determine which support channel performs best for response time, resolution and satisfaction.
### Task 4 — Priority Analysis
Compare Low, Medium, High and Critical tickets against SLA and resolution benchmarks.
### Task 5 — Customer Type
Compare New vs Existing customers by ticket count, CSAT, resolution time and escalation rate.
### Task 6 — Monthly Trend
Analyze monthly ticket volume, SLA compliance and CSAT.
### Task 7 — SLA Benchmark
Calculate SLA compliance rate by agent, issue and channel.
### Task 8 — Root-Cause Investigation
Find issue categories with high ticket volume and low satisfaction.
### Task 9 — Support Dashboard
Build KPI cards, slicers and charts for operational monitoring.
### Task 10 — Improvement Plan
Recommend actions to improve SLA compliance and CSAT.

---

## 7. Recommended Pivot Charts

1. **Tickets by Issue Category** — Bar Chart
2. **SLA Compliance by Agent** — Column Chart
3. **CSAT by Channel** — Column Chart
4. **Resolution Time by Priority** — Bar Chart
5. **Monthly Ticket Volume** — Line Chart
6. **Escalation Rate by Issue** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Total Tickets
- SLA Compliance
- Average Response Time
- Average Resolution Time
- Average CSAT
- Escalation Rate
- Reopen Rate
- High/Critical Tickets

### Filters / Slicers

- Agent
- Channel
- Issue_Category
- Priority
- Customer_Type

### Dashboard Charts

- Tickets by Issue
- SLA by Agent
- CSAT by Channel
- Monthly Ticket Trend

---

## 9. Final Business Questions

1. Which agent handles the most tickets?
2. Which agent has the best SLA compliance?
3. Which issue category creates the most tickets?
4. Which issue has the lowest CSAT?
5. Which channel is fastest?
6. Which priority has the worst SLA compliance?
7. Which categories exceed the resolution benchmark?
8. Which KPI requires immediate improvement?
9. What three service improvements should management implement?

---

## 10. Final Management Challenge

Management wants to improve customer experience without simply increasing headcount. Identify the main operational bottleneck and recommend three process changes.

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
