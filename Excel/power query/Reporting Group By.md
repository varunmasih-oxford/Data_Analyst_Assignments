Practice set **Power Query Group By**

### Dataset: Sales_Data

| Order_ID | Date       | Region | City      | Salesperson | Category    | Product | Quantity |  Sales | Profit |
| -------- | ---------- | ------ | --------- | ----------- | ----------- | ------- | -------: | -----: | -----: |
| 1001     | 01-01-2026 | North  | Delhi     | Amit        | Electronics | Laptop  |        2 | 120000 |  18000 |
| 1002     | 02-01-2026 | North  | Delhi     | Neha        | Furniture   | Chair   |        5 |  25000 |   5000 |
| 1003     | 03-01-2026 | West   | Mumbai    | Rahul       | Electronics | Mobile  |        4 |  80000 |  12000 |
| 1004     | 04-01-2026 | South  | Bangalore | Priya       | Electronics | Laptop  |        1 |  60000 |   9000 |
| 1005     | 05-01-2026 | East   | Kolkata   | Suresh      | Furniture   | Table   |        3 |  45000 |   7500 |
| 1006     | 06-01-2026 | North  | Noida     | Amit        | Electronics | Mobile  |        6 | 120000 |  18000 |
| 1007     | 07-01-2026 | West   | Pune      | Rahul       | Grocery     | Rice    |       20 |  20000 |   3000 |
| 1008     | 08-01-2026 | South  | Chennai   | Priya       | Grocery     | Oil     |       15 |  22500 |   3750 |
| 1009     | 09-01-2026 | East   | Kolkata   | Suresh      | Electronics | Laptop  |        2 | 120000 |  18000 |
| 1010     | 10-01-2026 | North  | Delhi     | Neha        | Grocery     | Rice    |       25 |  25000 |   4000 |
| 1011     | 11-01-2026 | West   | Mumbai    | Rahul       | Furniture   | Chair   |        8 |  40000 |   8000 |
| 1012     | 12-01-2026 | South  | Bangalore | Priya       | Electronics | Mobile  |        5 | 100000 |  15000 |
| 1013     | 13-01-2026 | East   | Patna     | Suresh      | Grocery     | Oil     |       10 |  15000 |   2500 |
| 1014     | 14-01-2026 | North  | Noida     | Amit        | Furniture   | Table   |        4 |  60000 |  10000 |
| 1015     | 15-01-2026 | West   | Pune      | Rahul       | Electronics | Laptop  |        3 | 180000 |  27000 |
| 1016     | 16-01-2026 | South  | Chennai   | Priya       | Furniture   | Chair   |        6 |  30000 |   6000 |
| 1017     | 17-01-2026 | East   | Patna     | Suresh      | Electronics | Mobile  |        7 | 140000 |  21000 |
| 1018     | 18-01-2026 | North  | Delhi     | Neha        | Grocery     | Oil     |       12 |  18000 |   3000 |
| 1019     | 19-01-2026 | West   | Mumbai    | Rahul       | Furniture   | Table   |        5 |  75000 |  12500 |
| 1020     | 20-01-2026 | South  | Bangalore | Priya       | Grocery     | Rice    |       30 |  30000 |   5000 |
| 1021     | 21-02-2026 | North  | Delhi     | Amit        | Electronics | Laptop  |        2 | 120000 |  18000 |
| 1022     | 22-02-2026 | North  | Noida     | Neha        | Furniture   | Chair   |       10 |  50000 |  10000 |
| 1023     | 23-02-2026 | West   | Mumbai    | Rahul       | Electronics | Mobile  |        3 |  60000 |   9000 |
| 1024     | 24-02-2026 | South  | Chennai   | Priya       | Electronics | Laptop  |        2 | 120000 |  18000 |
| 1025     | 25-02-2026 | East   | Kolkata   | Suresh      | Furniture   | Table   |        2 |  30000 |   5000 |
| 1026     | 26-02-2026 | North  | Delhi     | Amit        | Grocery     | Rice    |       40 |  40000 |   7000 |
| 1027     | 27-02-2026 | West   | Pune      | Rahul       | Electronics | Laptop  |        1 |  60000 |   9000 |
| 1028     | 28-02-2026 | South  | Bangalore | Priya       | Grocery     | Oil     |       20 |  30000 |   5000 |
| 1029     | 01-03-2026 | East   | Patna     | Suresh      | Electronics | Mobile  |        5 | 100000 |  15000 |
| 1030     | 02-03-2026 | North  | Noida     | Neha        | Furniture   | Table   |        3 |  45000 |   7500 |
| 1031     | 03-03-2026 | West   | Mumbai    | Rahul       | Grocery     | Rice    |       35 |  35000 |   6000 |
| 1032     | 04-03-2026 | South  | Chennai   | Priya       | Electronics | Mobile  |        8 | 160000 |  24000 |
| 1033     | 05-03-2026 | East   | Kolkata   | Suresh      | Grocery     | Oil     |       15 |  22500 |   3750 |
| 1034     | 06-03-2026 | North  | Delhi     | Amit        | Furniture   | Chair   |       12 |  60000 |  12000 |
| 1035     | 07-03-2026 | West   | Pune      | Rahul       | Electronics | Laptop  |        2 | 120000 |  18000 |
| 1036     | 08-03-2026 | South  | Bangalore | Priya       | Furniture   | Table   |        4 |  60000 |  10000 |
| 1037     | 09-03-2026 | East   | Patna     | Suresh      | Electronics | Mobile  |        6 | 120000 |  18000 |
| 1038     | 10-03-2026 | North  | Noida     | Neha        | Grocery     | Rice    |       30 |  30000 |   5000 |
| 1039     | 11-03-2026 | West   | Mumbai    | Rahul       | Furniture   | Chair   |        7 |  35000 |   7000 |
| 1040     | 12-03-2026 | South  | Chennai   | Priya       | Grocery     | Oil     |       25 |  37500 |   6250 |
| 1041     | 13-04-2026 | East   | Kolkata   | Suresh      | Electronics | Laptop  |        3 | 180000 |  27000 |
| 1042     | 14-04-2026 | North  | Delhi     | Amit        | Electronics | Mobile  |        8 | 160000 |  24000 |
| 1043     | 15-04-2026 | West   | Pune      | Rahul       | Grocery     | Rice    |       45 |  45000 |   8000 |
| 1044     | 16-04-2026 | South  | Bangalore | Priya       | Furniture   | Chair   |       10 |  50000 |  10000 |
| 1045     | 17-04-2026 | East   | Patna     | Suresh      | Grocery     | Oil     |       18 |  27000 |   4500 |
| 1046     | 18-04-2026 | North  | Noida     | Neha        | Electronics | Laptop  |        2 | 120000 |  18000 |
| 1047     | 19-04-2026 | West   | Mumbai    | Rahul       | Furniture   | Table   |        6 |  90000 |  15000 |
| 1048     | 20-04-2026 | South  | Chennai   | Priya       | Electronics | Mobile  |        9 | 180000 |  27000 |
| 1049     | 21-04-2026 | East   | Kolkata   | Suresh      | Furniture   | Chair   |        8 |  40000 |   8000 |
| 1050     | 22-04-2026 | North  | Delhi     | Amit        | Grocery     | Rice    |       50 |  50000 |   9000 |

## Practice Reports — Group By

Once you load this into **Power Query**, try creating these reports **without using PivotTable**.

### Level 1 — Basic Group By

1. **Total Sales by Region**

   * Region
   * Sum of Sales

2. **Total Profit by Category**

   * Category
   * Sum of Profit

3. **Total Quantity by Product**

   * Product
   * Sum of Quantity

4. **Number of Orders by Salesperson**

   * Salesperson
   * Count Rows

5. **Average Sales by Region**

   * Region
   * Average Sales

### Level 2 — Multiple Columns

6. **Sales by Region and Category**

   * Region
   * Category
   * Total Sales

7. **Profit by City and Product**

   * City
   * Product
   * Total Profit

8. **Quantity sold by Salesperson and Category**

   * Salesperson
   * Category
   * Total Quantity

9. **Sales and Profit by Region**

   * Region
   * Total Sales
   * Total Profit

### Level 3 — Business Reports

10. **Top-performing Salesperson**

* Salesperson
* Total Sales
* Total Profit
* Order Count

11. **City Performance Report**

* City
* Total Sales
* Total Profit
* Average Sales

12. **Product Performance Report**

* Product
* Total Quantity
* Total Sales
* Total Profit
* Average Sales

13. **Monthly Sales Report**

* Month
* Total Sales
* Total Profit
* Order Count

14. **Region + Category Performance**

* Region
* Category
* Total Sales
* Total Profit
* Total Quantity

15. **Best Product in Each Region**

* Region
* Product
* Total Sales
* Total Profit

### Level 4 — Advanced Power Query Practice

After basic Group By, try creating:

* **Highest-selling product**
* **Lowest-selling product**
* **Average order value**
* **Profit margin by category**
* **Top 3 cities by sales**
* **Top salesperson in each region**
* **Region-wise contribution to total sales**
* **Month-wise sales growth**
* **Category-wise profit ranking**
* **Salesperson performance comparison**
