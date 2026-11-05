# Sales Data Analyst – Practical Project

Retail Business Intelligence Solutions & Reporting | StoreTech UK

[storetech.com](<https://www.storetech.com/business-intelligence?utm_source=chatgpt.com>)

# Retail Sales Performance Analysis

Beginner to IntermediateHands-on ProjectData CleaningBusiness Analysis

Company: ABC Retail Store

Industry: Retail and E-commerce

Department: Sales and Business Intelligence

Your Role: Junior Data Analyst

Project: Sales Data Preparation and Performance Analysis

## 1. Business understanding

### Company background

ABC Retail Store is a retail company that sells products through online and physical stores across different regions.

The company sells four major product categories:

- Electronics
- Furniture
- Office Supplies
- Accessories

The business has been collecting sales data from different stores and online transactions.

However, management has noticed some problems:

- Monthly sales reports are inconsistent.
- Some customer records are duplicated.
- Certain orders have missing information.
- Product sales and profit calculations sometimes appear incorrect.
- Management cannot clearly identify the best-performing regions and products.

The company has hired you as a Data Analyst to investigate these problems.

### Your business objective

Your responsibility is to prepare the raw sales data and provide reliable insights to management.

Management wants answers to these questions:

1. What is the company's total revenue?
2. Which product category generates the highest sales?
3. Which region performs best?
4. Which products generate the highest profit?
5. Which month has the highest sales?
6. Which payment method is most commonly used?
7. How many orders are cancelled?
8. Are discounts affecting profitability?
9. Which customers contribute the most revenue?
10. What improvements can increase business performance?

## 2. Understand the dataset

You have received a raw sales dataset with the following columns.

| Column | Business meaning |
| --- | --- |
| Order\_ID | Unique order identification |
| Order\_Date | Date when order was placed |
| Customer\_ID | Unique customer identification |
| Customer\_Name | Name of customer |
| Region | Sales region |
| City | Customer city |
| Product | Product purchased |
| Category | Product category |
| Quantity | Number of units purchased |
| Unit\_Price | Price per unit |
| Discount | Discount percentage |
| Sales | Total sales amount |
| Cost | Total product cost |
| Profit | Sales minus cost |
| Order\_Status | Completed, Pending or Cancelled |
| Payment\_Mode | Payment method |

## 3. Raw sales dataset

Intentionally contains data quality issuesThe following sample contains 25 records. It includes missing values, duplicates, inconsistent formats, incorrect values, and business-rule issues.

You should clean the data rather than simply delete every suspicious record.

Dataset: abc\_retail\_raw.csv · 25 sample records

Raw dataset preview

CSV

Copy the data below into a file named `abc_retail_raw.csv`.

 Copy complete CSV dataset

## 4. Identify the data quality issues

Before cleaning, investigate these issues.

| Issue | Example | What you should do |
| --- | --- | --- |
| Missing values | Customer name is blank | Investigate and handle |
| Duplicate records | Order ID 1022 appears twice | Verify and remove accidental duplicate |
| Inconsistent dates | 05/01/2025 vs 2025-01-05 | Standardize dates |
| Inconsistent city | Delhi vs delhi | Standardize categories |
| Invalid quantity | -2 or 0 | Investigate business validity |
| Incorrect profit | Profit does not match Sales - Cost | Recalculate or investigate |
| Future date | 2027-04-01 | Verify against reporting period |
| Cancelled orders | Order 1013 | Define how cancellations affect sales |
| Discount formats | 10% and 0 | Standardize discount values |

Important: Some suspicious records might be valid business transactions. Document your assumptions before changing them.

## 5. Your practical data preparation tasks

Complete these tasks as if you are working for ABC Retail Store.

### Task 1: Data inspection

- Find total number of rows.
- Find total number of columns.
- Check column data types.
- Understand the meaning of each column.
- Identify the unique identifiers.

### Task 2: Missing value handling

- Find columns containing NULL values.
- Count missing values in each column.
- Decide how to handle missing customer names.
- Document your treatment.

### Task 3: Duplicate identification

- Identify duplicate Order IDs.
- Count duplicate records.
- Investigate whether the duplicates are exact duplicates.
- Remove accidental duplicates.

### Task 4: Data standardization

- Standardize date formats.
- Standardize city names.
- Standardize product categories.
- Standardize payment methods.
- Convert discounts into a consistent numerical format.

### Task 5: Data validation

Check the following business rules:

- Quantity should be positive for completed sales.
- Unit price should not be negative.
- Discount should be between 0% and 100%.
- Sales should be consistent with quantity, price, and discount.
- Profit should equal sales minus cost, subject to the company's accounting rules.
- Cancelled orders should not be counted as completed sales.
- Order dates should fall within the valid reporting period.

### Task 6: Data transformation

Create the following additional columns:

| New column | Calculation |
| --- | --- |
| Gross\_Sales | Quantity × Unit\_Price |
| Discount\_Amount | Gross\_Sales × Discount |
| Net\_Sales | Gross\_Sales - Discount\_Amount |
| Calculated\_Profit | Net\_Sales - Cost |
| Order\_Month | Extract month from Order\_Date |
| Order\_Year | Extract year from Order\_Date |

## 6. Business analysis tasks

Once your dataset is clean, answer these business questions.

| No. | Business question | Analysis required |
| --- | --- | --- |
| 1 | What is total revenue? | SUM of net sales |
| 2 | Which category sells the most? | Category-wise sales |
| 3 | Which region performs best? | Region-wise sales |
| 4 | Which product generates the most profit? | Product-wise profit |
| 5 | Which month has highest sales? | Monthly sales trend |
| 6 | Which payment method is most popular? | Payment count |
| 7 | What percentage of orders are cancelled? | Cancellation rate |
| 8 | Which customers generate the most revenue? | Customer ranking |
| 9 | Do discounts reduce profitability? | Discount vs profit analysis |
| 10 | Which products need improvement? | Sales and profit comparison |

## 7. Suggested dashboard design

After completing your analysis, build a Sales Performance Dashboard.

Power BI for Learners Part 12: Advanced Features, AI Capabilities, and the Future of Power BI | by David Marvellous | Power BI Masterclass | Mar, 2026 | Medium

[medium.com](<https://medium.com/microsoft-power-bi/power-bi-for-learners-part-12-advanced-features-ai-capabilities-and-the-future-of-power-bi-53f65d78532d?utm_source=chatgpt.com>)

Your dashboard should contain:

KPI Cards

- Total Revenue
- Total Profit
- Total Orders
- Average Order Value
- Cancellation Rate

Charts

- Monthly sales trend – Line chart
- Category-wise revenue – Bar chart
- Region-wise sales – Bar chart or map
- Top 5 products – Bar chart
- Payment method distribution – Donut chart
- Profit by category – Column chart

Filters

- Order Date
- Region
- Category
- Product
- Order Status

## 8. Tools to use for this project

| Tool | Practical assignment |
| --- | --- |
| Excel | Clean raw data and identify errors |
| SQL | Find duplicates, NULLs, and calculate sales |
| Python | Perform exploratory data analysis and cleaning |
| Power BI | Build an interactive sales dashboard |

## 9. Project deliverables

At the end of this project, you should have:

1. Raw sales dataset.
2. Data quality assessment.
3. Data cleaning documentation.
4. Cleaned sales dataset.
5. SQL queries or Python cleaning script.
6. Business analysis report.
7. Power BI sales dashboard.
8. Final business recommendations.

## 10. How to approach this project professionally

Follow this sequence:

| Phase | Your responsibility |
| --- | --- |
| Phase 1 | Understand the business |
| Phase 2 | Understand the dataset |
| Phase 3 | Inspect data quality |
| Phase 4 | Clean and transform data |
| Phase 5 | Validate business rules |
| Phase 6 | Perform business analysis |
| Phase 7 | Build dashboard |
| Phase 8 | Present insights to management |

## Final assignment: Think like a Data Analyst

Imagine your manager asks:

"Our sales are increasing, but our profit is not growing at the same rate. Can you investigate why?"

Use the dataset to investigate:

- Are discounts too high?
- Are some products generating low profit?
- Are certain regions underperforming?
- Are cancelled orders affecting reported sales?
- Are product costs increasing?

Your job is not just to produce numbers. Your job is to explain what is happening in the business and recommend what management should do.

Project success criteria: Your data should be clean, your calculations should be validated, and your recommendations should be supported by evidence.

## 5. Recommended learning sequence

I recommend completing this project in four stages rather than trying to do everything at once.

1. Stage 1 – Excel data preparation
   Clean the raw dataset, identify duplicates, missing values, invalid values, and standardize formats.
   Start here
2. Stage 2 – SQL data analysis
   Write queries using `SELECT`, `WHERE`, `GROUP BY`, `CASE WHEN`, `JOIN`, aggregate functions and window functions.
3. Stage 3 – Python data cleaning
   Use Pandas for missing values, duplicates, data types, outliers and validation.
4. Stage 4 – Power BI dashboard
   Build KPIs, charts, filters, and business insights.

My recommendation: Start by downloading or copying the raw CSV into Excel. Do not clean it immediately. First, inspect it and write down every issue you find. That is exactly how a real Data Analyst approaches a new business dataset.

Copied
