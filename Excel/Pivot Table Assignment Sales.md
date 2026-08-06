# Business Sales & Performance — Pivot Table Assignment

## 1. Dataset Overview

This dataset is designed for practicing:

- Excel Pivot Tables
- Pivot Charts
- Business KPI Analysis
- Industry Benchmarking
- Sales Performance Analysis
- Dashboard Creation
- Business Decision Making

### Dataset Columns

| Column | Description |
|---|---|
| Order_ID | Unique order number |
| Order_Date | Date of order |
| Region | Sales region |
| City | Customer city |
| Salesperson | Sales representative |
| Industry | Customer industry |
| Customer_Type | New or Existing |
| Product_Category | Product category |
| Product | Product name |
| Sales | Revenue generated |
| Cost | Cost of product/service |
| Profit | Sales - Cost |
| Units_Sold | Quantity sold |
| Discount_% | Discount percentage |
| Customer_Rating | Customer rating out of 5 |
| Delivery_Days | Number of days taken for delivery |
| Return_% | Percentage of returned items |

---

# 2. Business Sales Dataset

Save the following data as:

`business_sales_dataset.csv`

```csv
Order_ID,Order_Date,Region,City,Salesperson,Industry,Customer_Type,Product_Category,Product,Sales,Cost,Profit,Units_Sold,Discount_%,Customer_Rating,Delivery_Days,Return_%
ORD001,2026-01-05,North,Delhi,Rahul,Retail,New,Software,CRM Basic,85000,51000,34000,5,8,4.5,3,2
ORD002,2026-01-07,North,Noida,Priya,Education,Existing,Software,CRM Pro,125000,70000,55000,7,10,4.2,4,3
ORD003,2026-01-09,West,Mumbai,Amit,Healthcare,New,Hardware,POS System,95000,62000,33000,4,5,4.6,5,2
ORD004,2026-01-12,South,Bangalore,Neha,IT,Existing,Software,Analytics Pro,145000,80000,65000,8,12,4.7,3,1
ORD005,2026-01-15,East,Kolkata,Vikas,Retail,Existing,Services,Consulting,110000,65000,45000,2,5,4.1,7,4
ORD006,2026-01-18,North,Gurgaon,Rahul,Manufacturing,New,Hardware,Barcode Scanner,72000,48000,24000,6,7,4.3,4,3
ORD007,2026-01-21,West,Pune,Amit,Education,New,Software,LMS Basic,90000,54000,36000,10,10,4.4,3,2
ORD008,2026-01-24,South,Chennai,Neha,Healthcare,Existing,Services,Training,75000,42000,33000,3,4,4.8,6,1
ORD009,2026-01-27,East,Bhubaneswar,Vikas,IT,New,Software,Cloud Pro,135000,76000,59000,6,9,4.5,4,2
ORD010,2026-01-30,North,Delhi,Priya,Retail,Existing,Hardware,POS System,105000,68000,37000,5,6,4.0,5,4
ORD011,2026-02-03,West,Mumbai,Amit,IT,Existing,Software,Analytics Pro,160000,88000,72000,9,8,4.8,3,1
ORD012,2026-02-06,South,Bangalore,Neha,Manufacturing,New,Hardware,Barcode Scanner,80000,53000,27000,7,10,4.2,5,3
ORD013,2026-02-09,North,Noida,Rahul,Education,Existing,Services,Training,95000,55000,40000,4,5,4.6,6,2
ORD014,2026-02-12,East,Kolkata,Vikas,Healthcare,New,Software,CRM Pro,120000,69000,51000,6,11,4.3,4,3
ORD015,2026-02-15,West,Pune,Priya,Retail,New,Hardware,POS System,98000,64000,34000,5,7,4.1,5,4
ORD016,2026-02-18,South,Chennai,Neha,Education,Existing,Software,LMS Basic,87000,51000,36000,8,8,4.7,3,2
ORD017,2026-02-21,North,Gurgaon,Rahul,IT,New,Services,Consulting,150000,90000,60000,2,6,4.5,8,2
ORD018,2026-02-24,East,Bhubaneswar,Vikas,Manufacturing,Existing,Hardware,Barcode Scanner,76000,50000,26000,6,9,4.0,5,4
ORD019,2026-02-27,West,Mumbai,Amit,Healthcare,Existing,Software,Cloud Pro,140000,78000,62000,7,8,4.6,4,2
ORD020,2026-02-28,South,Bangalore,Neha,Retail,New,Services,Consulting,118000,70000,48000,2,5,4.2,7,3
ORD021,2026-03-03,North,Delhi,Priya,IT,Existing,Software,Analytics Pro,175000,95000,80000,10,10,4.9,3,1
ORD022,2026-03-06,East,Kolkata,Vikas,Education,New,Software,LMS Basic,92000,56000,36000,9,12,4.3,4,3
ORD023,2026-03-09,West,Pune,Amit,Manufacturing,Existing,Hardware,POS System,112000,73000,39000,5,6,4.4,5,3
ORD024,2026-03-12,South,Chennai,Neha,Healthcare,New,Services,Training,82000,46000,36000,4,5,4.7,6,1
ORD025,2026-03-15,North,Noida,Rahul,Retail,Existing,Software,CRM Basic,88000,53000,35000,5,8,4.0,3,3
ORD026,2026-03-18,East,Bhubaneswar,Vikas,IT,New,Software,Cloud Pro,155000,87000,68000,8,9,4.6,4,2
ORD027,2026-03-21,West,Mumbai,Priya,Education,Existing,Services,Training,100000,58000,42000,4,6,4.5,7,2
ORD028,2026-03-24,South,Bangalore,Neha,Manufacturing,New,Hardware,Barcode Scanner,85000,57000,28000,8,8,4.1,5,4
ORD029,2026-03-27,North,Gurgaon,Rahul,Healthcare,Existing,Software,CRM Pro,130000,74000,56000,7,10,4.4,4,2
ORD030,2026-03-30,East,Kolkata,Vikas,Retail,New,Hardware,POS System,102000,66000,36000,5,5,4.2,5,3
ORD031,2026-04-03,West,Pune,Amit,IT,Existing,Software,Analytics Pro,168000,92000,76000,9,8,4.8,3,1
ORD032,2026-04-06,South,Chennai,Neha,Education,New,Software,LMS Basic,94000,57000,37000,10,10,4.5,3,2
ORD033,2026-04-09,North,Delhi,Priya,Manufacturing,Existing,Hardware,Barcode Scanner,78000,52000,26000,6,7,4.0,5,4
ORD034,2026-04-12,East,Bhubaneswar,Vikas,Healthcare,New,Services,Consulting,125000,74000,51000,2,6,4.6,8,2
ORD035,2026-04-15,West,Mumbai,Amit,Retail,Existing,Software,CRM Basic,99000,59000,40000,6,9,4.3,3,3
ORD036,2026-04-18,South,Bangalore,Neha,IT,New,Software,Cloud Pro,148000,82000,66000,7,10,4.7,4,1
ORD037,2026-04-21,North,Noida,Rahul,Education,Existing,Services,Training,97000,56000,41000,4,5,4.4,6,2
ORD038,2026-04-24,East,Kolkata,Vikas,Manufacturing,New,Hardware,POS System,108000,71000,37000,5,8,4.1,5,3
ORD039,2026-04-27,West,Pune,Priya,Healthcare,Existing,Software,CRM Pro,138000,79000,59000,7,9,4.5,4,2
ORD040,2026-04-30,South,Chennai,Neha,Retail,New,Services,Consulting,122000,72000,50000,2,6,4.3,7,3
ORD041,2026-05-03,North,Delhi,Priya,IT,Existing,Software,Analytics Pro,182000,99000,83000,11,8,4.9,3,1
ORD042,2026-05-06,East,Kolkata,Vikas,Education,New,Software,LMS Basic,96000,58000,38000,10,11,4.2,4,3
ORD043,2026-05-09,West,Mumbai,Amit,Manufacturing,Existing,Hardware,Barcode Scanner,82000,55000,27000,7,7,4.3,5,3
ORD044,2026-05-12,South,Bangalore,Neha,Healthcare,New,Services,Training,88000,49000,39000,4,4,4.8,6,1
ORD045,2026-05-15,North,Gurgaon,Rahul,Retail,Existing,Software,CRM Basic,93000,56000,37000,6,9,4.1,3,3
ORD046,2026-05-18,East,Bhubaneswar,Vikas,IT,New,Software,Cloud Pro,162000,90000,72000,8,8,4.7,4,2
ORD047,2026-05-21,West,Pune,Priya,Education,Existing,Services,Training,103000,60000,43000,5,5,4.6,6,2
ORD048,2026-05-24,South,Chennai,Neha,Manufacturing,New,Hardware,POS System,115000,75000,40000,6,7,4.2,5,3
ORD049,2026-05-27,North,Noida,Rahul,Healthcare,Existing,Software,CRM Pro,135000,77000,58000,7,10,4.5,4,2
ORD050,2026-05-30,East,Kolkata,Vikas,Retail,New,Hardware,Barcode Scanner,79000,52000,27000,6,6,4.0,5,4
````

---

# 3. Business Scenario

You are working as a **Business Data Analyst** for a company that sells:

* Software
* Hardware
* Business Services

Management wants to analyze business performance across:

* Regions
* Cities
* Industries
* Products
* Salespeople
* Customer types
* Months

The management team also wants to compare actual performance against predefined **business benchmarks**.

Your job is to create a **Pivot Table-based Business Performance Report**.

---

# 4. Industry / Business Benchmarks

Use the following benchmarks for the analysis.

| KPI                      |      Benchmark |
| ------------------------ | -------------: |
| Profit Margin            |  35% or higher |
| Customer Rating          |  4.3 or higher |
| Delivery Days            | 5 days or less |
| Return Rate              |     3% or less |
| Discount                 |    10% or less |
| Salesperson Sales Target |      ₹4,50,000 |
| Regional Sales Target    |     ₹12,00,000 |
| Average Order Value      |      ₹1,00,000 |

---

# 5. Important Formulas

## Profit Margin

```text
Profit Margin = Profit / Sales × 100
```

In Excel:

```excel
=Profit/Sales*100
```

---

## Average Order Value

```text
Average Order Value = Total Sales / Number of Orders
```

In Excel:

```excel
=Total Sales/Total Orders
```

---

# 6. Assignment Tasks

## Task 1 — Regional Performance

Create a Pivot Table.

### Rows

* Region

### Values

* Sum of Sales
* Sum of Cost
* Sum of Profit
* Average Customer Rating
* Average Delivery Days
* Average Return %

### Questions

1. Which region has the highest sales?
2. Which region has the highest profit?
3. Which region has the highest customer rating?
4. Which region has the lowest delivery time?
5. Which region has the highest return rate?
6. Which region is performing best overall?

Compare each region against the business benchmarks.

---

# 7. Task 2 — Industry Performance

Create a Pivot Table.

### Rows

* Industry

### Values

* Sum of Sales
* Sum of Profit
* Average Customer Rating
* Average Delivery Days
* Average Return %

Calculate:

```text
Profit Margin %
```

### Questions

1. Which industry generates the highest revenue?
2. Which industry generates the highest profit?
3. Which industry has the highest profit margin?
4. Which industry has the best customer rating?
5. Which industry has the highest return rate?
6. Which industries are above the 35% profit-margin benchmark?
7. Which industries are below the benchmark?

---

# 8. Task 3 — Salesperson Performance

Create a Pivot Table.

### Rows

* Salesperson

### Values

* Sum of Sales
* Sum of Profit
* Count of Order_ID
* Average Customer Rating

Sort the Pivot Table by:

```text
Sales → Largest to Smallest
```

## Sales Target

Each salesperson has a sales target of:

```text
₹4,50,000
```

Classify each salesperson as:

```text
Above Target
Below Target
```

### Questions

1. Who generated the highest sales?
2. Who generated the highest profit?
3. Who received the highest customer rating?
4. Who achieved the sales target?
5. Who needs improvement?

---

# 9. Task 4 — Product Performance

Create a Pivot Table.

### Rows

* Product

### Values

* Sum of Sales
* Sum of Profit
* Sum of Units Sold
* Average Discount %
* Average Customer Rating
* Average Return %

### Questions

1. Which product has the highest sales?
2. Which product has the highest profit?
3. Which product has the highest units sold?
4. Which product has the highest return rate?
5. Which product has the best customer rating?
6. Which product should management promote more aggressively?

---

# 10. Task 5 — Customer Type Analysis

Create a Pivot Table.

### Rows

* Customer_Type

### Values

* Count of Order_ID
* Sum of Sales
* Sum of Profit
* Average Customer Rating
* Average Discount %

Compare:

* New Customers
* Existing Customers

### Questions

1. Which customer type generates more sales?
2. Which customer type generates more profit?
3. Which customer type receives higher discounts?
4. Which customer type has better ratings?
5. Which customer type should the company focus on?

---

# 11. Task 6 — Monthly Sales Analysis

Create a Pivot Table.

### Rows

* Order_Date

Group the date field by:

```text
Months
```

### Values

* Sum of Sales
* Sum of Profit
* Count of Order_ID

Create a:

**Line Chart**

### Questions

1. Which month generated the highest sales?
2. Which month generated the highest profit?
3. Which month had the most orders?
4. Is sales performance improving over time?

---

# 12. Task 7 — Region × Product Category

Create a Pivot Table.

### Rows

* Region

### Columns

* Product_Category

### Values

* Sum of Sales

Create a:

**Stacked Column Chart**

### Questions

1. Which product category performs best in each region?
2. Which region generates the highest software sales?
3. Which region generates the highest hardware sales?
4. Which region generates the highest services sales?

---

# 13. Task 8 — Benchmark Gap Analysis

Create a separate summary table.

| KPI                 | Actual | Benchmark | Status |
| ------------------- | -----: | --------: | ------ |
| Profit Margin       |      — |       35% | —      |
| Customer Rating     |      — |       4.3 | —      |
| Delivery Days       |      — |         5 | —      |
| Return Rate         |      — |        3% | —      |
| Discount            |      — |       10% | —      |
| Average Order Value |      — | ₹1,00,000 | —      |

---

## Benchmark Status

For metrics where **higher is better**:

```excel
=IF(B2>=C2,"Above Benchmark","Below Benchmark")
```

For metrics where **lower is better**:

```excel
=IF(B4<=C4,"Within Benchmark","Above Benchmark")
```

---

# 14. Task 9 — Regional Sales Target

Regional sales target:

```text
₹12,00,000
```

Create a Pivot Table:

### Rows

* Region

### Values

* Sum of Sales

Add a calculated/status column:

```text
Target Achieved
Target Not Achieved
```

### Questions

1. Which regions achieved the sales target?
2. Which regions failed to achieve the target?
3. What is the sales gap for underperforming regions?

---

# 15. Task 10 — Business Performance Dashboard

Create a one-page dashboard using Pivot Tables and Pivot Charts.

## KPI Cards

Display:

* Total Sales
* Total Profit
* Profit Margin %
* Total Orders
* Average Order Value
* Average Customer Rating
* Average Delivery Days
* Return Rate

---

## Recommended Charts

### Chart 1

**Sales by Region**

Chart Type:

```text
Column Chart
```

---

### Chart 2

**Profit by Industry**

Chart Type:

```text
Bar Chart
```

---

### Chart 3

**Monthly Sales Trend**

Chart Type:

```text
Line Chart
```

---

### Chart 4

**Sales by Product**

Chart Type:

```text
Bar Chart
```

---

### Chart 5

**Salesperson Performance**

Chart Type:

```text
Column Chart
```

---

### Chart 6

**Region × Product Category**

Chart Type:

```text
Stacked Column Chart
```

---

# 16. Recommended Dashboard Filters

Add Pivot Table Slicers for:

* Region
* Industry
* Customer_Type
* Product_Category
* Product
* Salesperson

Add a Timeline for:

* Order_Date

---

# 17. Final Management Questions

After completing the analysis, answer the following questions.

## Sales Performance

1. Which region is the strongest?
2. Which region has the highest sales?
3. Which region has the highest profit?
4. Which industry generates the highest revenue?
5. Which product is the most profitable?
6. Who is the best-performing salesperson?

## Benchmark Analysis

7. Is the overall profit margin above 35%?
8. Is the average customer rating above 4.3?
9. Is average delivery time within 5 days?
10. Is the return rate within 3%?
11. Is the average discount within 10%?
12. Is the average order value above ₹1,00,000?

## Management Decisions

13. Which region should receive additional investment?
14. Which product should be promoted?
15. Which salesperson requires additional support?
16. Which industry segment should the company target?
17. Which KPI needs immediate improvement?
18. What three actions would you recommend to management?

---

# 18. Final Deliverable

Create an Excel workbook with the following sheets:

### Sheet 1 — Raw Data

Store the complete dataset.

### Sheet 2 — Regional Analysis

Regional Pivot Table and analysis.

### Sheet 3 — Industry Analysis

Industry-wise Pivot Table.

### Sheet 4 — Salesperson Analysis

Salesperson performance Pivot Table.

### Sheet 5 — Product Analysis

Product performance Pivot Table.

### Sheet 6 — Customer Analysis

New vs Existing customer analysis.

### Sheet 7 — Monthly Analysis

Monthly sales and profit analysis.

### Sheet 8 — Benchmark Analysis

Actual vs benchmark comparison.

### Sheet 9 — Dashboard

Create a professional management dashboard.

---

# 19. Skills Being Tested

Students will be evaluated on their ability to use:

* Excel Tables
* Pivot Tables
* Pivot Charts
* Slicers
* Timeline
* Grouping
* Sorting
* Filtering
* Calculated Fields
* Percentage calculations
* KPI analysis
* Benchmark analysis
* Conditional Formatting
* Dashboard Design
* Business Insights
* Data-driven Decision Making

---

# 20. Challenge Task

Management has asked:

> "If you were the Business Manager, what would you change based on this data?"

Write a short management report containing:

### 1. Top 3 Findings

Identify the three most important findings from your analysis.

### 2. Top 3 Problems

Identify three areas performing below expectations.

### 3. Top 3 Recommendations

Suggest three practical business actions.

### 4. Management Summary

Write a **5–7 sentence executive summary** explaining the overall business performance.

---
