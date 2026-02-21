## Topic: Aggregation Functions

### Objective
Practice and understand how Aggregation Functions work in DAX for totals and summarization.

Functions Covered:
- SUM
- AVERAGE
- MIN
- MAX
- COUNT
- DISTINCTCOUNT

---

# Dataset Used

Tables:
- Sales
- Customers
- Products
- Regions

Make sure relationships are properly created before starting.

---

# Part 1: Basic Aggregations

### Q1. Create a measure to calculate Total Sales Amount.
Use:
SUM()

Expected Measure Name:
Total Sales

---

### Q2. Create a measure to calculate Average Sales per Order.
Use:
AVERAGE()

Expected Measure Name:
Average Sales

---

### Q3. Find the Minimum Sale Amount recorded.
Use:
MIN()

Expected Measure Name:
Minimum Sale

---

### Q4. Find the Maximum Sale Amount recorded.
Use:
MAX()

Expected Measure Name:
Maximum Sale

---

# Part 2: Counting Functions

### Q5. Count total number of orders.
Use:
COUNT()

Expected Measure Name:
Total Orders

---

### Q6. Count total number of unique customers.
Use:
DISTINCTCOUNT()

Expected Measure Name:
Unique Customers

---

# Part 3: Visual Based Tasks

Create the following visuals:

1. Card Visual – Show Total Sales
2. Card Visual – Show Total Orders
3. Table Visual – Show:
   - Customer Name
   - Total Sales
4. Bar Chart – Region vs Total Sales
5. Column Chart – Product Category vs Average Sales

---

# Part 4: Conceptual Questions

1. What is the difference between COUNT and DISTINCTCOUNT?
2. Why do we prefer SUM over manual addition?
3. What happens if there are blank values in AVERAGE?
4. Can MIN and MAX work on text columns?
5. What is the difference between COUNT and COUNTROWS?

---

# Challenge Task (Bonus)

1. Create a measure:
   Average Sales Per Customer

2. Create a measure:
   Total Sales Per Region

3. Sort customers by Total Sales (Descending).

---
