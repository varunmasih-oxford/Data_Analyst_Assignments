# Excel Practical Assignment: Conditional Formatting & Statistical Functions

## Objective

Learn how to analyze business sales data using Excel's statistical functions and Conditional Formatting.

### Statistical Functions Covered

- `SUM()`
- `COUNT()`
- `COUNTA()`
- `AVERAGE()`
- `MIN()`
- `MAX()`

### Conditional Formatting Covered

- Highlight Cell Rules
- Top/Bottom Rules
- Duplicate Values
- Data Bars
- Color Scales
- Icon Sets
- Formula-Based Conditional Formatting

---

# Dataset

Enter the following data into Excel.

| Order ID | Salesperson | Region | Product | Units Sold | Unit Price | Sales Amount | Target Sales |
|----------|-------------|---------|----------|-----------:|-----------:|-------------:|-------------:|
| ORD001 | Aditi | North | Laptop | 8 | 55000 | 440000 | 400000 |
| ORD002 | Rahul | South | Printer | 15 | 12000 | 180000 | 200000 |
| ORD003 | Neha | East | Monitor | 12 | 18000 | 216000 | 220000 |
| ORD004 | Arjun | West | Keyboard | 30 | 1500 | 45000 | 50000 |
| ORD005 | Kavya | North | Mouse | 45 | 700 | 31500 | 40000 |
| ORD006 | Mohit | South | Laptop | 6 | 55000 | 330000 | 350000 |
| ORD007 | Priya | East | Printer | 18 | 12000 | 216000 | 200000 |
| ORD008 | Rohan | West | Monitor | 10 | 18000 | 180000 | 180000 |
| ORD009 | Sneha | North | Laptop | 9 | 55000 | 495000 | 450000 |
| ORD010 | Aman | South | Keyboard | 40 | 1500 | 60000 | 55000 |

---

# Part A: Statistical Functions

Perform the following calculations.

## Question 1

Find the **Total Sales Amount** using the `SUM()` function.

---

## Question 2

Count the total number of orders using the `COUNT()` function.

---

## Question 3

Count the total number of salespersons using the `COUNTA()` function.

---

## Question 4

Find the **Average Sales Amount** using the `AVERAGE()` function.

---

## Question 5

Find the **Highest Sales Amount** using the `MAX()` function.

---

## Question 6

Find the **Lowest Sales Amount** using the `MIN()` function.

---

## Question 7

Calculate the **Total Units Sold**.

---

## Question 8

Find the **Average Unit Price**.

---

## Question 9

Find the **Highest Unit Price**.

---

## Question 10

Find the **Lowest Unit Price**.

---

# Part B: Business Analysis

Create the following columns.

## Question 11

Create a **Sales Difference** column.

**Formula**

Sales Amount − Target Sales

---

## Question 12

Create a **Target Status** column.

Display:

- Achieved
- Not Achieved

based on Sales Amount.

---

## Question 13

Calculate the **Performance Percentage**.

Formula:

Performance % = (Sales Amount ÷ Target Sales) × 100

---

## Question 14

Create a **Bonus Eligibility** column.

Display:

- Eligible
- Not Eligible

if Sales Amount is greater than Target Sales.

---

## Question 15

Calculate **Commission**.

- 5% if Sales Amount is above Target Sales
- 2% otherwise

---

# Part C: Conditional Formatting

Apply the following Conditional Formatting rules.

## Question 16

Highlight the **Highest Sales Amount** using a **Green Fill**.

---

## Question 17

Highlight the **Lowest Sales Amount** using a **Red Fill**.

---

## Question 18

Highlight Sales Amounts greater than **₹300,000**.

---

## Question 19

Highlight Sales Amounts less than **₹100,000**.

---

## Question 20

Highlight **Duplicate Product Names**.

---

## Question 21

Highlight the **Top 3 Sales Amounts**.

---

## Question 22

Highlight the **Bottom 3 Sales Amounts**.

---

## Question 23

Apply **Data Bars** to the Sales Amount column.

---

## Question 24

Apply **Green-Yellow-Red Color Scales** to Sales Amount.

---

## Question 25

Apply **Icon Sets** to the Performance % column.

---

# Part D: Formula-Based Conditional Formatting

Use Conditional Formatting formulas.

## Question 26

Highlight the entire row if:

Sales Amount ≥ Target Sales

---

## Question 27

Highlight the entire row if:

Sales Amount < Target Sales

---

## Question 28

Highlight all rows where Product = **Laptop**.

---

## Question 29

Highlight all rows where Region = **North**.

---

## Question 30

Apply Alternate Row Colors using Conditional Formatting formulas.

---

# Part E: Summary Dashboard

Using statistical functions, create the following summary table.

| Metric | Value |
|---------|-------|
| Total Orders | |
| Total Sales | |
| Total Units Sold | |
| Average Sales | |
| Highest Sale | |
| Lowest Sale | |
| Highest Unit Price | |
| Lowest Unit Price | |
| Number of Salespersons | |
| Average Unit Price | |

---

# Part F: Practical Challenges

## Question 31

Find how many sales exceeded the target.

---

## Question 32

Find how many sales failed to meet the target.

---

## Question 33

Find the salesperson with the **Highest Sales Amount**.

---

## Question 34

Find the salesperson with the **Lowest Sales Amount**.

---

## Question 35

Find the **Average Sales Amount** for all **Laptop** orders.

---

## Question 36

Find the **Total Sales** made in the **North** region.

---

## Question 37

Find the **Highest Sales Amount** in the **South** region.

---

## Question 38

Find the **Lowest Sales Amount** in the **West** region.

---

## Question 39

Create a **Performance Rating**.

Display:

- Excellent if Performance ≥ 120%
- Good if Performance ≥ 100%
- Average if Performance ≥ 80%
- Poor otherwise

---

## Question 40

Create the following summary using text concatenation.

Example Output:

> Aditi sold Laptop worth ₹440000

---

# Bonus Practice

## Bonus 1

Highlight all Sales Amounts greater than the Average Sales.

---

## Bonus 2

Highlight Odd-numbered Order IDs using Formula-Based Conditional Formatting.

---

## Bonus 3

Highlight Even-numbered Order IDs.

---

## Bonus 4

Apply a Color Scale showing:

- Green = High Sales
- Yellow = Medium Sales
- Red = Low Sales

---

## Bonus 5

Calculate the percentage of salespersons who achieved their targets.

---

## Bonus 6

Find the Product with the maximum total sales.

---

## Bonus 7

Create a KPI section displaying:

- Highest Sale
- Lowest Sale
- Average Sale
- Target Achievement %
- Total Revenue

---
