**Consolidating and Enriching Sales Data Using Merge and Append in Power Query**

## Business Problem

ABC Electronics is a nationwide retailer that sells laptops, mobile phones, and computer accessories through branches located in Delhi, Mumbai, Bengaluru, and Chennai.

Every month, each branch sends its sales data to the Head Office in separate Excel files. The company also maintains separate master tables for products, customers, and sales employees.

The management team faces the following challenges:

* Sales data is stored in multiple files, making it difficult to prepare consolidated reports.
* The sales files contain only Product IDs and Customer IDs, making the reports difficult to understand.
* Management wants to analyze sales by product category, customer location, and salesperson performance.
* Preparing monthly reports manually is time-consuming and prone to errors.

To solve these issues, the Business Intelligence team decides to use **Power Query**.

---

# Objectives

The objective of this assignment is to:

1. Combine sales data from multiple branch files.
2. Add product and customer information to the sales data.
3. Create a clean and consolidated dataset for reporting.
4. Generate insights that support business decision-making.

---

# Available Datasets

### Table 1: Delhi Sales

| Invoice No | Date   | Product ID | Customer ID | Salesperson ID | Quantity | Sales Amount |
| ---------- | ------ | ---------- | ----------- | -------------- | -------- | ------------ |
| 1001       | 01-Jan | P101       | C001        | S001           | 2        | 80,000       |
| 1002       | 02-Jan | P205       | C005        | S002           | 1        | 1,000        |

---

### Table 2: Mumbai Sales

| Invoice No | Date   | Product ID | Customer ID | Salesperson ID | Quantity | Sales Amount |
| ---------- | ------ | ---------- | ----------- | -------------- | -------- | ------------ |
| 1003       | 03-Jan | P103       | C003        | S003           | 1        | 45,000       |
| 1004       | 04-Jan | P205       | C002        | S001           | 3        | 3,000        |

---

### Table 3: Product Master

| Product ID | Product Name   | Category    | Cost Price |
| ---------- | -------------- | ----------- | ---------- |
| P101       | Laptop         | Electronics | 35,000     |
| P103       | Tablet         | Electronics | 30,000     |
| P205       | Wireless Mouse | Accessories | 600        |

---

### Table 4: Customer Master

| Customer ID | Customer Name | City      | Customer Segment |
| ----------- | ------------- | --------- | ---------------- |
| C001        | Rahul Sharma  | Delhi     | Corporate        |
| C002        | Anita Singh   | Mumbai    | Retail           |
| C003        | Vikas Kumar   | Bengaluru | Corporate        |
| C005        | Priya Mehta   | Delhi     | Retail           |

---

### Table 5: Salesperson Master

| Salesperson ID | Salesperson Name | Region |
| -------------- | ---------------- | ------ |
| S001           | Amit Verma       | North  |
| S002           | Neha Gupta       | North  |
| S003           | Rohan Patel      | West   |

---

# Tasks

## Task 1: Append Queries

Use **Append Queries** to combine the Delhi Sales and Mumbai Sales tables into a single **Master Sales** table.

**Expected Outcome:**
A single table containing all sales transactions from both branches.

---

## Task 2: Merge with Product Master

Merge the Master Sales table with the Product Master using **Product ID**.

Expand the following columns:

* Product Name
* Category
* Cost Price

---

## Task 3: Merge with Customer Master

Merge the updated Sales table with the Customer Master using **Customer ID**.

Expand the following columns:

* Customer Name
* City
* Customer Segment

---

## Task 4: Merge with Salesperson Master

Merge the Sales table with the Salesperson Master using **Salesperson ID**.

Expand:

* Salesperson Name
* Region

---

## Task 5: Create New Columns

Create the following calculated columns:

* **Total Cost = Quantity × Cost Price**
* **Profit = Sales Amount − Total Cost**

---

# Expected Final Dataset

The final table should contain:

* Invoice Number
* Date
* Product Name
* Category
* Customer Name
* City
* Customer Segment
* Salesperson Name
* Region
* Quantity
* Sales Amount
* Cost Price
* Total Cost
* Profit

---

# Business Questions

Use the final dataset to answer the following questions:

1. Which product category generated the highest sales?
2. Which city generated the highest revenue?
3. Who is the top-performing salesperson?
4. Which customer segment contributes the most revenue?
5. What is the total profit earned by the company?
6. Which products have the highest profit margins?
7. Which region achieved the highest sales?
8. What are the top five products by sales amount?

---

# Business Benefits

After implementing Merge and Append in Power Query, ABC Electronics will be able to:

* Consolidate sales data from multiple branches automatically.
* Eliminate manual copying and reduce reporting errors.
* Produce faster monthly sales reports.
* Analyze customer purchasing patterns.
* Measure salesperson performance accurately.
* Monitor product profitability.
* Support management with timely, data-driven decision-making.

