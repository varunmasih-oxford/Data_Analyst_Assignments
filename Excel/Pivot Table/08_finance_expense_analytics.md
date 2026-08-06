# Project 8: Finance & Expense Analytics

## 1. Business Scenario

The finance team wants to monitor department budgets, actual spending, vendor costs and approval status to control unnecessary expenses.

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
| Expense_ID | Expense identifier |
| Month | Expense month |
| Department | Department |
| Expense_Category | Expense category |
| Vendor | Vendor |
| Budget | Approved budget amount |
| Actual_Expense | Actual expense |
| Payment_Method | Payment method |
| Approval_Status | Approval status |
| Cost_Center | Cost center |
| Recurring | Yes/No |
| Variance_Reason | Reason for variance |

---

## 3. Dataset

Save the following data as:

`08_finance_expense_analytics.csv`

```csv
Expense_ID,Month,Department,Expense_Category,Vendor,Budget,Actual_Expense,Payment_Method,Approval_Status,Cost_Center,Recurring,Variance_Reason
EXP001,2026-01,HR,Software,Vendor D,106999,83240,UPI,Rejected,CC-106,Yes,Underspend
EXP002,2026-02,Marketing,Utilities,Vendor D,178611,218553,Card,Approved,CC-102,No,Overspend
EXP003,2026-03,Marketing,Training,Vendor C,104822,120263,Bank Transfer,Rejected,CC-106,No,Overspend
EXP004,2026-04,Sales,Software,Vendor D,267748,280671,Card,Approved,CC-101,Yes,Within Budget
EXP005,2026-05,Operations,Advertising,Vendor D,136088,137633,Bank Transfer,Rejected,CC-101,Yes,Within Budget
EXP006,2026-06,Operations,Travel,Vendor A,279492,335615,Bank Transfer,Pending,CC-106,Yes,Overspend
EXP007,2026-01,Finance,Advertising,Vendor D,30629,36708,UPI,Pending,CC-103,Yes,Overspend
EXP008,2026-02,IT,Professional Fees,Vendor D,254896,220419,Card,Rejected,CC-106,Yes,Underspend
EXP009,2026-03,IT,Professional Fees,Vendor B,253078,206749,Bank Transfer,Pending,CC-105,No,Underspend
EXP010,2026-04,Finance,Advertising,Vendor A,165164,139482,UPI,Rejected,CC-101,Yes,Underspend
EXP011,2026-05,Finance,Professional Fees,Vendor C,226623,244134,Card,Pending,CC-101,Yes,Within Budget
EXP012,2026-06,HR,Office,Vendor D,253384,272587,UPI,Pending,CC-105,No,Within Budget
EXP013,2026-01,IT,Training,Vendor D,238380,268770,Bank Transfer,Pending,CC-105,No,Overspend
EXP014,2026-02,Operations,Office,Vendor D,163052,202878,UPI,Approved,CC-106,Yes,Overspend
EXP015,2026-03,Finance,Software,Vendor A,150466,146448,Bank Transfer,Rejected,CC-104,No,Within Budget
EXP016,2026-04,Finance,Travel,Vendor A,57290,47571,Bank Transfer,Pending,CC-105,No,Underspend
EXP017,2026-05,Marketing,Office,Vendor A,76211,59600,UPI,Approved,CC-106,No,Underspend
EXP018,2026-06,Operations,Office,Vendor A,240053,253731,Bank Transfer,Rejected,CC-104,No,Within Budget
EXP019,2026-01,Finance,Professional Fees,Vendor C,35615,30303,Bank Transfer,Approved,CC-105,Yes,Underspend
EXP020,2026-02,HR,Software,Vendor A,118857,129199,Bank Transfer,Approved,CC-103,No,Overspend
EXP021,2026-03,IT,Training,Vendor B,215140,233390,UPI,Approved,CC-106,Yes,Overspend
EXP022,2026-04,Finance,Professional Fees,Vendor C,77272,79188,Card,Pending,CC-102,Yes,Within Budget
EXP023,2026-05,Operations,Travel,Vendor C,268424,326096,Bank Transfer,Pending,CC-105,Yes,Overspend
EXP024,2026-06,HR,Travel,Vendor C,67951,68058,UPI,Rejected,CC-103,No,Within Budget
EXP025,2026-01,Marketing,Professional Fees,Vendor C,227698,234889,Card,Rejected,CC-104,Yes,Within Budget
EXP026,2026-02,Sales,Utilities,Vendor B,282691,228452,UPI,Rejected,CC-102,No,Underspend
EXP027,2026-03,Operations,Training,Vendor A,246229,302300,UPI,Pending,CC-102,No,Overspend
EXP028,2026-04,Finance,Professional Fees,Vendor C,78763,74782,Bank Transfer,Rejected,CC-102,No,Within Budget
EXP029,2026-05,Operations,Office,Vendor B,194559,180311,UPI,Rejected,CC-102,No,Within Budget
EXP030,2026-06,Marketing,Professional Fees,Vendor C,134682,116827,Bank Transfer,Approved,CC-102,Yes,Underspend
EXP031,2026-01,Sales,Travel,Vendor A,216660,179393,UPI,Rejected,CC-104,Yes,Underspend
EXP032,2026-02,HR,Training,Vendor C,52158,61233,Card,Rejected,CC-103,No,Overspend
EXP033,2026-03,Operations,Office,Vendor D,125877,156364,Bank Transfer,Rejected,CC-102,Yes,Overspend
EXP034,2026-04,Operations,Travel,Vendor C,251866,249135,Card,Rejected,CC-102,No,Within Budget
EXP035,2026-05,IT,Office,Vendor A,93107,102335,Bank Transfer,Rejected,CC-102,No,Overspend
EXP036,2026-06,Operations,Professional Fees,Vendor C,82820,75591,Bank Transfer,Rejected,CC-103,Yes,Underspend
EXP037,2026-01,Operations,Office,Vendor C,171247,168793,Bank Transfer,Pending,CC-104,Yes,Within Budget
EXP038,2026-02,HR,Office,Vendor D,249725,274786,Card,Pending,CC-102,Yes,Overspend
EXP039,2026-03,Finance,Office,Vendor B,149834,173372,UPI,Pending,CC-104,Yes,Overspend
EXP040,2026-04,Finance,Software,Vendor D,106464,122435,Bank Transfer,Approved,CC-104,No,Overspend
EXP041,2026-05,Finance,Training,Vendor C,100501,125403,Card,Pending,CC-103,Yes,Overspend
EXP042,2026-06,Marketing,Travel,Vendor B,238877,190979,Card,Pending,CC-106,Yes,Underspend
EXP043,2026-01,HR,Office,Vendor C,265853,298365,UPI,Rejected,CC-103,No,Overspend
EXP044,2026-02,HR,Professional Fees,Vendor B,40399,38616,UPI,Rejected,CC-106,Yes,Within Budget
EXP045,2026-03,Finance,Training,Vendor D,179216,166232,UPI,Pending,CC-101,No,Within Budget
EXP046,2026-04,Marketing,Professional Fees,Vendor B,180220,176953,UPI,Pending,CC-104,No,Within Budget
EXP047,2026-05,HR,Software,Vendor C,67404,53219,Card,Rejected,CC-103,No,Underspend
EXP048,2026-06,IT,Professional Fees,Vendor C,237332,210186,UPI,Rejected,CC-105,No,Underspend
EXP049,2026-01,Sales,Software,Vendor B,247049,205954,UPI,Pending,CC-106,Yes,Underspend
EXP050,2026-02,Sales,Travel,Vendor A,140400,117017,Card,Rejected,CC-101,Yes,Underspend
EXP051,2026-03,Sales,Travel,Vendor C,238148,241003,UPI,Approved,CC-101,No,Within Budget
EXP052,2026-04,Finance,Office,Vendor D,192199,166190,UPI,Approved,CC-102,Yes,Underspend
EXP053,2026-05,HR,Professional Fees,Vendor C,44979,34524,Card,Pending,CC-105,No,Underspend
EXP054,2026-06,Finance,Training,Vendor B,263226,215202,UPI,Rejected,CC-104,No,Underspend
EXP055,2026-01,IT,Training,Vendor B,192351,231679,Bank Transfer,Pending,CC-103,No,Overspend
EXP056,2026-02,HR,Travel,Vendor A,246113,216555,UPI,Approved,CC-103,No,Underspend
EXP057,2026-03,Finance,Utilities,Vendor D,275994,280837,Card,Approved,CC-104,No,Within Budget
EXP058,2026-04,Operations,Office,Vendor B,151223,173662,Card,Rejected,CC-104,No,Overspend
EXP059,2026-05,Finance,Advertising,Vendor D,161017,133907,Card,Approved,CC-103,Yes,Underspend
EXP060,2026-06,Operations,Professional Fees,Vendor C,251375,267126,Card,Rejected,CC-106,No,Within Budget
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| Budget Variance | Within ±5% |
| Overspend Rate | 10% or lower |
| Pending Approval | 5% or lower |
| Recurring Expense Growth | 5% or lower |
| Budget Utilization | 90%–100% |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **Budget Variance**: `Actual Expense − Budget`
- **Variance %**: `(Actual Expense − Budget) / Budget × 100`
- **Budget Utilization**: `Actual Expense / Budget × 100`
- **Overspend Rate**: `Overspent records / Total records × 100`
- **Pending Approval Rate**: `Pending records / Total records × 100`

---

## 6. Assignment Tasks

### Task 1 — Department Budget Analysis
Compare Budget, Actual Expense and Variance by Department.
### Task 2 — Expense Category Analysis
Identify categories with the highest actual expense and largest unfavorable variance.
### Task 3 — Vendor Analysis
Compare vendors by total spend, transaction count and average expense.
### Task 4 — Monthly Expense Trend
Analyze budget vs actual expense by month.
### Task 5 — Cost Center Analysis
Compare spending across cost centers.
### Task 6 — Recurring Expense Analysis
Compare recurring vs non-recurring expenses and identify high recurring-cost categories.
### Task 7 — Approval Analysis
Analyze Approved, Pending and Rejected expenses by department.
### Task 8 — Benchmark Analysis
Classify departments/categories against budget variance and overspend benchmarks.
### Task 9 — Finance Dashboard
Build KPI cards, slicers and charts for budget monitoring.
### Task 10 — Cost Control Recommendations
Identify where management can reduce unnecessary spending.

---

## 7. Recommended Pivot Charts

1. **Budget vs Actual by Department** — Clustered Column Chart
2. **Variance by Expense Category** — Bar Chart
3. **Monthly Budget vs Actual** — Line/Column Chart
4. **Vendor Spend** — Bar Chart
5. **Recurring vs Non-Recurring** — Column Chart
6. **Approval Status** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Total Budget
- Actual Expense
- Variance
- Variance %
- Budget Utilization
- Overspend Rate
- Pending Approval Rate
- Recurring Spend

### Filters / Slicers

- Department
- Expense_Category
- Vendor
- Month
- Approval_Status
- Recurring

### Dashboard Charts

- Budget vs Actual
- Variance by Category
- Monthly Budget vs Actual
- Vendor Spend

---

## 9. Final Business Questions

1. Which department has the highest spending?
2. Which department has the largest unfavorable variance?
3. Which expense category causes the most overspending?
4. Which vendor receives the most money?
5. Which month has the highest variance?
6. Which departments are within the ±5% benchmark?
7. What percentage of expenses are pending?
8. Which recurring expenses should be reviewed?
9. What three cost-control recommendations should management implement?

---

## 10. Final Management Challenge

The CFO wants to reduce unnecessary costs while protecting business-critical operations. Identify the departments and expense categories where action would have the greatest impact.

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
