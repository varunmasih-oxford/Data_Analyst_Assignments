
# Power Query Assignment: Date, Time & Duration Practice Set

## Dataset: Sales_Data

**Total Records:** 30  
**Total Columns:** 12

## Objective

Practice Date, Time and Duration transformations in Power Query using one combined Sales_Data dataset.

Skills covered:

- Date extraction and calculations
- Time extraction and calculations
- Duration transformations
- Date and Time combination
- Delivery time analysis
- Business reporting
- Conditional columns
- Date-based business keys

---

# Part 1: Combined Sales_Data Dataset

Copy this dataset into Excel and convert it into an Excel Table named `Sales_Data`.

| Order_ID | Date | Time | Region | City | Salesperson | Category | Product | Sales | Delivery_Date | Delivery_Time | Processing_Duration |
|---|---|---|---|---|---|---|---|---:|---|---|---|
| 1001 | 01-01-2026 | 09:15:00 | North | Delhi | Amit | Electronics | Laptop | 55000 | 03-01-2026 | 12:15:00 | 03:00:00 |
| 1002 | 02-01-2026 | 10:30:00 | West | Mumbai | Neha | Electronics | Mobile | 25000 | 05-01-2026 | 15:30:00 | 05:30:00 |
| 1003 | 03-01-2026 | 14:45:00 | South | Bangalore | Rahul | Furniture | Chair | 5000 | 08-01-2026 | 16:45:00 | 02:15:00 |
| 1004 | 04-01-2026 | 16:20:00 | East | Kolkata | Priya | Furniture | Table | 12000 | 10-01-2026 | 18:20:00 | 04:00:00 |
| 1005 | 05-01-2026 | 11:10:00 | North | Delhi | Suresh | Grocery | Rice | 2000 | 07-01-2026 | 14:10:00 | 06:00:00 |
| 1006 | 10-02-2026 | 18:30:00 | West | Mumbai | Amit | Grocery | Oil | 1500 | 15-02-2026 | 20:30:00 | 02:00:00 |
| 1007 | 15-02-2026 | 08:45:00 | South | Chennai | Neha | Electronics | Laptop | 52000 | 18-02-2026 | 13:45:00 | 04:30:00 |
| 1008 | 20-03-2026 | 12:30:00 | East | Patna | Rahul | Furniture | Chair | 4500 | 25-03-2026 | 17:30:00 | 03:15:00 |
| 1009 | 25-03-2026 | 15:15:00 | North | Noida | Priya | Electronics | Mobile | 22000 | 30-03-2026 | 16:15:00 | 05:00:00 |
| 1010 | 01-04-2026 | 19:00:00 | West | Pune | Suresh | Grocery | Rice | 1800 | 04-04-2026 | 21:00:00 | 02:30:00 |
| 1011 | 12-04-2026 | 07:30:00 | North | Delhi | Amit | Furniture | Table | 15000 | 14-04-2026 | 10:30:00 | 03:00:00 |
| 1012 | 18-04-2026 | 13:20:00 | South | Bangalore | Neha | Grocery | Oil | 1700 | 24-04-2026 | 16:20:00 | 03:00:00 |
| 1013 | 22-04-2026 | 09:45:00 | East | Kolkata | Rahul | Electronics | Mobile | 24000 | 26-04-2026 | 12:45:00 | 03:00:00 |
| 1014 | 05-05-2026 | 17:10:00 | West | Mumbai | Priya | Furniture | Chair | 6000 | 12-05-2026 | 20:10:00 | 03:00:00 |
| 1015 | 11-05-2026 | 11:50:00 | North | Noida | Suresh | Electronics | Laptop | 58000 | 13-05-2026 | 14:50:00 | 03:00:00 |
| 1016 | 15-06-2026 | 06:45:00 | South | Chennai | Amit | Grocery | Rice | 2200 | 19-06-2026 | 09:45:00 | 03:00:00 |
| 1017 | 20-06-2026 | 14:10:00 | East | Patna | Neha | Furniture | Table | 13000 | 23-06-2026 | 17:10:00 | 03:00:00 |
| 1018 | 25-06-2026 | 20:15:00 | West | Pune | Rahul | Electronics | Mobile | 26000 | 03-07-2026 | 23:15:00 | 03:00:00 |
| 1019 | 02-07-2026 | 10:00:00 | North | Delhi | Priya | Grocery | Oil | 1900 | 04-07-2026 | 13:00:00 | 03:00:00 |
| 1020 | 10-07-2026 | 15:40:00 | South | Bangalore | Suresh | Electronics | Laptop | 56000 | 16-07-2026 | 18:40:00 | 03:00:00 |
| 1021 | 15-07-2026 | 08:20:00 | East | Kolkata | Amit | Furniture | Chair | 5500 | 18-07-2026 | 11:20:00 | 03:00:00 |
| 1022 | 20-08-2026 | 12:00:00 | West | Mumbai | Neha | Grocery | Rice | 2100 | 25-08-2026 | 15:00:00 | 03:00:00 |
| 1023 | 25-08-2026 | 16:30:00 | North | Noida | Rahul | Electronics | Mobile | 23000 | 02-09-2026 | 19:30:00 | 03:00:00 |
| 1024 | 05-09-2026 | 09:10:00 | South | Chennai | Priya | Furniture | Table | 14000 | 08-09-2026 | 12:10:00 | 03:00:00 |
| 1025 | 12-09-2026 | 18:45:00 | East | Patna | Suresh | Grocery | Oil | 1600 | 15-09-2026 | 21:45:00 | 03:00:00 |
| 1026 | 01-10-2026 | 07:15:00 | North | Delhi | Amit | Electronics | Laptop | 59000 | 04-10-2026 | 10:15:00 | 03:00:00 |
| 1027 | 10-10-2026 | 13:50:00 | West | Pune | Neha | Furniture | Chair | 6500 | 14-10-2026 | 16:50:00 | 03:00:00 |
| 1028 | 20-10-2026 | 21:10:00 | South | Bangalore | Rahul | Grocery | Rice | 2300 | 28-10-2026 | 00:10:00 | 03:00:00 |
| 1029 | 05-11-2026 | 10:40:00 | East | Kolkata | Priya | Electronics | Mobile | 27000 | 09-11-2026 | 13:40:00 | 03:00:00 |
| 1030 | 10-11-2026 | 15:25:00 | North | Noida | Suresh | Furniture | Table | 16000 | 13-11-2026 | 18:25:00 | 03:00:00 |

---

# Part 2: Data Types

| Column | Data Type |
|---|---|
| Order_ID | Whole Number |
| Date | Date |
| Time | Time |
| Region | Text |
| City | Text |
| Salesperson | Text |
| Category | Text |
| Product | Text |
| Sales | Whole Number |
| Delivery_Date | Date |
| Delivery_Time | Time |
| Processing_Duration | Duration |

**Important:** Set the correct data types before starting the exercises. Use Change Type → Using Locale if date formats are interpreted incorrectly.

---

# Part 3: Level 1 — Date Transformations

### Task 1: Extract Year

Use Date → Year → Year.

Create: `Order_Year`

### Task 2: Extract Month Number

Use Date → Month → Month.

Create: `Order_Month`

### Task 3: Extract Month Name

Use Date → Month → Name of Month.

Create: `Month_Name`

### Task 4: Extract Day of Month

Use Date → Day → Day.

Create: `Order_Day`

### Task 5: Extract Day Name

Use Date → Day → Name of Day.

Create: `Day_Name`

### Task 6: Extract Day of Week

Use Date → Day → Day of Week.

Create: `Day_Of_Week`

Note: Sunday = 0.

### Task 7: Extract Quarter

Use Date → Quarter → Quarter of Year.

Create: `Order_Quarter`

### Task 8: Extract Start of Month

Use Date → Month → Start of Month.

Create: `Month_Start_Date`

### Task 9: Extract End of Month

Use Date → Month → End of Month.

Create: `Month_End_Date`

### Task 10: Extract Start of Year

Use Date → Year → Start of Year.

Create: `Year_Start_Date`

---

# Part 4: Level 2 — Date Calculations

### Task 11: Add 7 Days

Create: `Date_After_7_Days`

### Task 12: Subtract 10 Days

Create: `Date_Before_10_Days`

### Task 13: Add 3 Months

Create: `Date_After_3_Months`

### Task 14: Add 1 Year

Create: `Date_After_1_Year`

### Task 15: Calculate Days Between Order and Delivery

Use:

- Date
- Delivery_Date

Create: `Delivery_Days`

Calculate:

`Delivery_Date - Date`

### Task 16: Calculate Days Until Month End

Create: `Days_To_Month_End`

Calculate:

`Month_End_Date - Date`

### Task 17: Create Financial Quarter

Create: `Financial_Quarter`

Expected values:

- Q1
- Q2
- Q3
- Q4

### Task 18: Create Year-Month

Create: `Year_Month`

Example: `2026-01`

---

# Part 5: Level 3 — Time Transformations

### Task 19: Extract Hour

Use Time → Hour.

Create: `Order_Hour`

### Task 20: Extract Minute

Use Time → Minute.

Create: `Order_Minute`

### Task 21: Extract Second

Use Time → Second.

Create: `Order_Second`

### Task 22: Extract Start of Hour

Use Time → Start of Hour.

Create: `Hour_Start`

### Task 23: Extract Start of Minute

Use Time → Start of Minute.

Create: `Minute_Start`

### Task 24: Extract End of Hour

Use Time → End of Hour.

Create: `Hour_End`

### Task 25: Create Time Category

Create: `Time_Category`

Conditions:

- Before 12:00 = Morning
- 12:00 to 17:00 = Afternoon
- After 17:00 = Evening

---

# Part 6: Level 4 — Duration Transformations

Use `Processing_Duration`.

### Task 26: Extract Duration Days

Create: `Duration_Days`

### Task 27: Extract Total Hours

Create: `Total_Hours`

### Task 28: Extract Total Minutes

Create: `Total_Minutes`

### Task 29: Extract Total Seconds

Create: `Total_Seconds`

### Task 30: Extract Duration Hours Component

Create: `Duration_Hours`

### Task 31: Extract Duration Minutes Component

Create: `Duration_Minutes`

### Task 32: Extract Duration Seconds Component

Create: `Duration_Seconds`

### Task 33: Add Two Durations

Create two additional duration columns:

- Processing_Time
- Shipping_Time

Add both columns.

Create: `Total_Duration`

---

# Part 7: Level 5 — Combined Date, Time and Duration Transformations

### Task 34: Create Order DateTime

Combine:

- Date
- Time

Create: `Order_DateTime`

### Task 35: Create Delivery DateTime

Combine:

- Delivery_Date
- Delivery_Time

Create: `Delivery_DateTime`

### Task 36: Calculate Processing Duration

Calculate:

`Delivery_DateTime - Order_DateTime`

Create: `Calculated_Processing_Duration`

### Task 37: Calculate Processing Hours

Convert duration into total hours.

Create: `Processing_Hours`

### Task 38: Create Delivery Status

Create: `Delivery_Status`

Conditions:

- Delivery within 3 days = On Time
- Delivery after 3 days = Delayed

### Task 39: Create Weekend or Weekday

Create: `Day_Type`

Conditions:

- Saturday or Sunday = Weekend
- Monday to Friday = Weekday

### Task 40: Create Order Age

Use a fixed reporting date of 14-11-2026.

Calculate:

`Reporting_Date - Date`

Create: `Order_Age_Days`

---

# Part 8: Level 6 — Business Reporting Practice

### Task 41: Create Order Month Label

Combine:

- Month_Name
- Order_Year

Create: `Order_Month_Label`

Example: January 2026

### Task 42: Create Order Period

Combine:

- Order_Year
- Order_Quarter

Create: `Order_Period`

Example: 2026-Q1

### Task 43: Create Working Day Flag

Create: `Working_Day_Flag`

### Task 44: Create Delivery Performance Category

Use Delivery_Days.

Conditions:

- 0–2 days = Excellent
- 3–5 days = Good
- 6–7 days = Average
- More than 7 days = Poor

Create: `Delivery_Performance`

### Task 45: Create Time Slot

Create: `Time_Slot`

Conditions:

- 06:00–11:59 = Morning Shift
- 12:00–17:59 = Afternoon Shift
- 18:00–23:59 = Evening Shift
- 00:00–05:59 = Night Shift

### Task 46: Create Order Processing Category

Use Processing_Hours.

Conditions:

- Up to 2 hours = Fast
- More than 2 up to 5 hours = Normal
- More than 5 up to 8 hours = Slow
- More than 8 hours = Very Slow

Create: `Processing_Category`

### Task 47: Create Monthly Sales Period

Create: `Sales_Period`

Example: Jan-2026

### Task 48: Create Date-Based Business Key

Combine:

- Order Year
- Order Month
- Order Day
- Order_ID

Create: `Date_Business_Key`

Example: `2026_01_01_1001`

---

# Part 9: Level 7 — Advanced Combined Challenges

### Challenge 1: Create Order Aging Category

Create: `Order_Aging_Category`

Conditions:

- 0–7 days = Recent
- 8–15 days = Moderate
- 16–30 days = Old
- More than 30 days = Very Old

### Challenge 2: Create Delivery Time in Hours

Calculate the difference between Order_DateTime and Delivery_DateTime.

Create: `Delivery_Time_Hours`

### Challenge 3: Create Monthly Order Code

Combine:

- Year
- Month Number
- Order_ID

Create: `Monthly_Order_Code`

Example: `202601_1001`

### Challenge 4: Create Week Number

Use Date → Week → Week of Year.

Create: `Order_Week_Number`

### Challenge 5: Create Complete Order Timeline

Combine:

- Order_DateTime
- Delivery_DateTime
- Processing_Duration

Create: `Order_Timeline`

### Challenge 6: Create Business Reporting Calendar

Create:

1. Calendar_Year
2. Calendar_Quarter
3. Month_Number
4. Month_Name
5. Week_Number
6. Day_Name
7. Day_Type
8. Month_Start_Date
9. Month_End_Date
10. Year_Start_Date

### Challenge 7: Create Complete Delivery Performance Report

Use:

- Order_ID
- Order_Date
- Delivery_Date
- Delivery_Days
- Delivery_Status
- Delivery_Performance

Sort Delivery_Days in descending order.

---

# Part 10: Submission Requirements

For every task:

1. Load Sales_Data into Power Query.
2. Create a duplicate query or reference query for practice.
3. Use the appropriate Date, Time or Duration transformation.
4. Rename columns clearly.
5. Keep original columns unchanged wherever possible.
6. Apply transformations in the correct order.
7. Check data types.
8. Load final results back into Excel.
9. Keep exercises in separate queries where appropriate.
10. Do not manually modify the original source dataset.

---

# Power Query Skills Covered

## Date Transformations

- Year
- Month
- Month Name
- Day
- Day Name
- Day of Week
- Quarter
- Start of Month
- End of Month
- Start of Year
- Week of Year

## Date Calculations

- Add Days
- Subtract Days
- Add Months
- Add Years
- Calculate Date Differences
- Calculate Days Until Month End

## Time Transformations

- Hour
- Minute
- Second
- Start of Hour
- Start of Minute
- End of Hour
- Time Classification

## Duration Transformations

- Days
- Hours
- Minutes
- Seconds
- Total Hours
- Total Minutes
- Total Seconds
- Add Durations

## Combined Skills

- Date and Time Combination
- DateTime Creation
- Duration Calculation
- Delivery Performance Analysis
- Order Aging Analysis
- Monthly Reporting
- Quarterly Reporting
- Business Calendar Creation
- Conditional Columns
- Business Reporting Preparation

---

# Final Objective

Develop practical Power Query skills in preparing date-based reports, analyzing delivery timelines, calculating processing durations, and creating business reporting columns.

**Total Practice: 48 Tasks + 7 Advanced Challenges**

**Dataset: Sales_Data (30 Records)**
