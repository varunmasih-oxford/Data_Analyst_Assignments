Assignment: Power Query — Date, Time & Duration Column Practice Set

## Dataset: Sales\_Data

| Order\_ID | Date | Time | Region | City | Salesperson | Category | Product | Sales | Delivery\_Date | Delivery\_Time | Processing\_Duration |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
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

## Data types to apply in Power Query

| Column | Data Type |
| --- | --- |
| Order\_ID | Whole Number |
| Date | Date |
| Time | Time |
| Region | Text |
| City | Text |
| Salesperson | Text |
| Category | Text |
| Product | Text |
| Sales | Whole Number |
| Delivery\_Date | Date |
| Delivery\_Time | Time |
| Processing\_Duration | Duration |

Objective

Practice the following Power Query Date, Time and Duration Column options:

Date transformations
Time transformations
Duration transformations
Extracting date and time components
Calculating date differences
Calculating time differences
Creating business reporting columns
Combining Date, Time and Duration transformations

Important: Complete all exercises using Power Query transformations. Do not manually edit the source data.

Level 1 — Date Transformations
Task 1: Extract Year from Date

Use the Date column.

Apply:

Transform → Date → Year → Year

Create a new column:

Order_Year

Expected result:

Date	Order_Year
01-01-2026	2026
15-02-2026	2026
20-03-2025	2025
Task 2: Extract Month Number

Use the Date column.

Apply:

Transform → Date → Month → Month

Create:

Order_Month

Expected result:

Date	Order_Month
01-01-2026	1
15-02-2026	2
20-03-2025	3
Task 3: Extract Month Name

Use:

Transform → Date → Month → Name of Month

Create:

Month_Name

Expected result:

Date	Month_Name
01-01-2026	January
15-02-2026	February
20-03-2025	March
Task 4: Extract Day of Month

Use:

Transform → Date → Day → Day

Create:

Order_Day

Expected result:

Date	Order_Day
01-01-2026	1
15-02-2026	15
20-03-2025	20
Task 5: Extract Day Name

Use:

Transform → Date → Day → Name of Day

Create:

Day_Name

Expected result:

Date	Day_Name
01-01-2026	Thursday
02-01-2026	Friday
03-01-2026	Saturday
Task 6: Extract Day of Week

Use:

Transform → Date → Day → Day of Week

Create:

Day_Of_Week

Expected result:

Date	Day_Of_Week
01-01-2026	3
02-01-2026	4
03-01-2026	5

Note: Power Query numbers weekdays starting with Sunday = 0.

Task 7: Extract Quarter of Year

Use:

Transform → Date → Quarter → Quarter of Year

Create:

Order_Quarter

Expected result:

Date	Order_Quarter
15-01-2026	1
15-04-2026	2
15-07-2026	3
15-10-2026	4
Task 8: Extract Start of Month

Use:

Transform → Date → Month → Start of Month

Create:

Month_Start_Date

Expected result:

Date	Month_Start_Date
15-01-2026	01-01-2026
20-02-2026	01-02-2026
25-03-2026	01-03-2026
Task 9: Extract End of Month

Use:

Transform → Date → Month → End of Month

Create:

Month_End_Date

Expected result:

Date	Month_End_Date
15-01-2026	31-01-2026
20-02-2026	28-02-2026
25-03-2026	31-03-2026
Task 10: Extract Start of Year

Use:

Transform → Date → Year → Start of Year

Create:

Year_Start_Date

Expected result:

Date	Year_Start_Date
15-01-2026	01-01-2026
20-06-2026	01-01-2026
25-03-2025	01-01-2025
Level 2 — Date Calculations
Task 11: Add Days to Date

Use:

Add Column → Date → Add Days

Add 7 days to the Date column.

Create:

Date_After_7_Days

Expected result:

Date	Date_After_7_Days
01-01-2026	08-01-2026
15-02-2026	22-02-2026
25-12-2025	01-01-2026
Task 12: Subtract Days from Date

Subtract 10 days from the Date column.

Create:

Date_Before_10_Days

Expected result:

Date	Date_Before_10_Days
15-01-2026	05-01-2026
10-02-2026	31-01-2026
Task 13: Add Months to Date

Add 3 months to the Date column.

Create:

Date_After_3_Months

Expected result:

Date	Date_After_3_Months
15-01-2026	15-04-2026
10-02-2026	10-05-2026
20-11-2025	20-02-2026
Task 14: Add Years to Date

Add 1 year to the Date column.

Create:

Date_After_1_Year

Expected result:

Date	Date_After_1_Year
15-01-2026	15-01-2027
20-06-2025	20-06-2026
Task 15: Calculate Days Between Dates

Create a custom column using two date columns:

Order_Date
Delivery_Date

Calculate the difference.

Create:

Delivery_Days

Expected result:

Order_Date	Delivery_Date	Delivery_Days
01-01-2026	05-01-2026	4
10-02-2026	15-02-2026	5
20-03-2026	28-03-2026	8
Task 16: Calculate Days Until Month End

Use:

Date → End of Month

Then calculate the difference between:

Date
Month_End_Date

Create:

Days_To_Month_End

Expected result:

Date	Month_End_Date	Days_To_Month_End
01-01-2026	31-01-2026	30
15-02-2026	28-02-2026	13
20-03-2026	31-03-2026	11
Task 17: Create Financial Quarter

Use the Date column.

Create a custom column that displays:

Q1
Q2
Q3
Q4

Create:

Financial_Quarter

Expected result:

Date	Financial_Quarter
15-01-2026	Q1
15-04-2026	Q2
15-07-2026	Q3
15-10-2026	Q4
Task 18: Create Year-Month Column

Combine the year and month from the Date column.

Create:

Year_Month

Expected result:

Date	Year_Month
15-01-2026	2026-01
20-02-2026	2026-02
25-03-2025	2025-03
Level 3 — Time Transformations

For these exercises, use a Time column if available. Otherwise, create a practice Time column using the example values below.

Example Time values:

09:15:30, 10:30:45, 14:45:20, 16:20:10

Task 19: Extract Hour

Use:

Transform → Time → Hour

Create:

Order_Hour

Expected result:

Time	Order_Hour
09:15:30	9
10:30:45	10
14:45:20	14
16:20:10	16
Task 20: Extract Minute

Use:

Transform → Time → Minute

Create:

Order_Minute

Expected result:

Time	Order_Minute
09:15:30	15
10:30:45	30
14:45:20	45
16:20:10	20
Task 21: Extract Second

Use:

Transform → Time → Second

Create:

Order_Second

Expected result:

Time	Order_Second
09:15:30	30
10:30:45	45
14:45:20	20
16:20:10	10
Task 22: Extract Start of Hour

Use:

Transform → Time → Start of Hour

Create:

Hour_Start

Expected result:

Time	Hour_Start
09:15:30	09:00:00
10:30:45	10:00:00
14:45:20	14:00:00
Task 23: Extract Start of Minute

Use:

Transform → Time → Start of Minute

Create:

Minute_Start

Expected result:

Time	Minute_Start
09:15:30	09:15:00
10:30:45	10:30:00
14:45:20	14:45:00
Task 24: Extract End of Hour

Use:

Transform → Time → End of Hour

Create:

Hour_End

Expected result:

Time	Hour_End
09:15:30	09:59:59
10:30:45	10:59:59
14:45:20	14:59:59
Task 25: Create Time Category

Use the Hour column.

Create a custom column:

Time_Category

Apply the following conditions:

Before 12:00 PM = Morning
12:00 PM to 5:00 PM = Afternoon
After 5:00 PM = Evening

Expected result:

Time	Time_Category
09:15:30	Morning
14:45:20	Afternoon
18:30:00	Evening
Level 4 — Duration Transformations

For these exercises, create a practice Duration column or use the duration values provided.

Example Duration values:

00:30:00, 01:15:30, 02:45:00, 03:20:15

Task 26: Extract Total Days from Duration

Use a Duration column.

Apply:

Transform → Duration → Days

Create:

Duration_Days

Expected result:

Duration	Duration_Days
1.00:00:00	1
2.00:00:00	2
3.00:00:00	3
Task 27: Extract Total Hours

Use:

Transform → Duration → Total Hours

Create:

Total_Hours

Expected result:

Duration	Total_Hours
00:30:00	0.5
01:15:30	1.2583
02:45:00	2.75
Task 28: Extract Total Minutes

Use:

Transform → Duration → Total Minutes

Create:

Total_Minutes

Expected result:

Duration	Total_Minutes
00:30:00	30
01:15:00	75
02:45:00	165
Task 29: Extract Total Seconds

Use:

Transform → Duration → Total Seconds

Create:

Total_Seconds

Expected result:

Duration	Total_Seconds
00:01:00	60
00:05:00	300
01:00:00	3600
Task 30: Extract Duration Hours Component

Use:

Transform → Duration → Hours

Create:

Duration_Hours

Expected result:

Duration	Duration_Hours
01:30:00	1
02:45:00	2
03:20:15	3
Task 31: Extract Duration Minutes Component

Use:

Transform → Duration → Minutes

Create:

Duration_Minutes

Expected result:

Duration	Duration_Minutes
01:30:00	30
02:45:00	45
03:20:15	20
Task 32: Extract Duration Seconds Component

Use:

Transform → Duration → Seconds

Create:

Duration_Seconds

Expected result:

Duration	Duration_Seconds
01:30:15	15
02:45:30	30
03:20:45	45
Task 33: Add Two Durations

Create two practice columns:

Processing_Duration
Shipping_Duration

Add both duration columns.

Create:

Total_Duration

Expected result:

Processing_Duration	Shipping_Duration	Total_Duration
00:30:00	01:00:00	01:30:00
01:15:00	02:00:00	03:15:00
02:30:00	00:45:00	03:15:00
Level 5 — Combined Date, Time and Duration Transformations
Task 34: Create Order DateTime

Combine:

Date
Time

Create a Date/Time column:

Order_DateTime

Example:

Date	Time	Order_DateTime
01-01-2026	09:15:00	01-01-2026 09:15:00
02-01-2026	10:30:00	02-01-2026 10:30:00
Task 35: Create Delivery DateTime

Combine:

Delivery_Date
Delivery_Time

Create:

Delivery_DateTime

Example:

Delivery_Date	Delivery_Time	Delivery_DateTime
05-01-2026	14:30:00	05-01-2026 14:30:00
Task 36: Calculate Order Processing Time

Calculate the difference between:

Order_DateTime
Delivery_DateTime

Create:

Processing_Duration

Expected result:

Order_DateTime	Delivery_DateTime	Processing_Duration
01-01-2026 09:00	01-01-2026 12:00	03:00:00
02-01-2026 10:00	02-01-2026 15:30	05:30:00
Task 37: Calculate Order Completion Hours

Use the Processing_Duration column.

Apply:

Duration → Total Hours

Create:

Processing_Hours

Expected result:

Processing_Duration	Processing_Hours
03:00:00	3
05:30:00	5.5
08:15:00	8.25
Task 38: Create Delivery Status

Use:

Order_Date
Delivery_Date

Create a conditional column:

Delivery_Status

Conditions:

Delivery_Date is before or equal to Order_Date + 3 days = On Time
Delivery_Date is greater than Order_Date + 3 days = Delayed

Expected result:

Order_Date	Delivery_Date	Delivery_Status
01-01-2026	03-01-2026	On Time
01-01-2026	04-01-2026	On Time
01-01-2026	06-01-2026	Delayed
Task 39: Create Weekend or Weekday Classification

Use the Date column.

Create:

Day_Type

Conditions:

Saturday or Sunday = Weekend
Monday to Friday = Weekday

Expected result:

Date	Day_Name	Day_Type
01-01-2026	Thursday	Weekday
03-01-2026	Saturday	Weekend
04-01-2026	Sunday	Weekend
Task 40: Create Order Age

Use the Date column and a fixed reporting date of 14-11-2026.

Calculate the number of days between:

Date
Reporting_Date

Create:

Order_Age_Days

Expected result:

Date	Reporting_Date	Order_Age_Days
01-11-2026	14-11-2026	13
05-11-2026	14-11-2026	9
10-11-2026	14-11-2026	4
Level 6 — Business Reporting Practice
Task 41: Create Order Month Label

Use:

Month Name
Year

Create:

Order_Month_Label

Example:

January 2026

February 2026

March 2026

Task 42: Create Order Period

Create a custom column using:

Year
Quarter

Create:

Order_Period

Expected result:

Date	Order_Period
15-01-2026	2026-Q1
15-04-2026	2026-Q2
15-07-2026	2026-Q3
Task 43: Create Working Day Flag

Use the Date column.

Create:

Working_Day_Flag

Conditions:

Monday to Friday = Working Day
Saturday and Sunday = Non-Working Day
Task 44: Create Delivery Performance Category

Use the Delivery_Days column.

Create:

Delivery_Performance

Conditions:

0 to 2 days = Excellent
3 to 5 days = Good
6 to 7 days = Average
More than 7 days = Poor
Task 45: Create Time Slot

Use the Time column.

Create:

Time_Slot

Conditions:

06:00 to 11:59 = Morning Shift
12:00 to 17:59 = Afternoon Shift
18:00 to 23:59 = Evening Shift
00:00 to 05:59 = Night Shift
Task 46: Create Order Processing Category

Use Processing_Hours.

Create:

Processing_Category

Conditions:

Less than or equal to 2 hours = Fast
More than 2 and up to 5 hours = Normal
More than 5 and up to 8 hours = Slow
More than 8 hours = Very Slow
Task 47: Create Monthly Sales Period

Use the Date column.

Create:

Sales_Period

Expected result:

Date	Sales_Period
01-01-2026	Jan-2026
15-02-2026	Feb-2026
20-03-2026	Mar-2026
Task 48: Create Date-Based Business Key

Create:

Date_Business_Key

Combine:

Order Year
Order Month
Order Day
Order ID

Example:

2026_01_01_1001

Level 7 — Advanced Combined Challenges
Challenge 1: Create Order Aging Category

Use the Order_Age_Days column.

Create:

Order_Aging_Category

Conditions:

0 to 7 days = Recent
8 to 15 days = Moderate
16 to 30 days = Old
More than 30 days = Very Old
Challenge 2: Create Delivery Time in Hours

Use:

Order_DateTime
Delivery_DateTime

Calculate the difference.

Create:

Delivery_Time_Hours

Convert the duration into total hours.

Challenge 3: Create Monthly Order Code

Create:

Monthly_Order_Code

Use:

Year
Month Number
Order_ID

Example:

202601_1001

Challenge 4: Create Week Number

Use the Date column.

Apply:

Transform → Date → Week → Week of Year

Create:

Order_Week_Number

Expected result:

Date	Order_Week_Number
01-01-2026	1
15-02-2026	7
20-03-2026	12

Note: Week numbering can vary depending on the week-start convention.

Challenge 5: Create Complete Order Timeline

Create a column:

Order_Timeline

Combine:

Order_DateTime
Delivery_DateTime
Processing_Duration

Example:

01-01-2026 09:00 | 01-01-2026 12:00 | 03:00:00

Apply appropriate formatting.

Challenge 6: Create Business Reporting Calendar

Create the following columns from the Date column:

Calendar_Year
Calendar_Quarter
Month_Number
Month_Name
Week_Number
Day_Name
Day_Type
Month_Start_Date
Month_End_Date
Year_Start_Date
Challenge 7: Create Complete Delivery Performance Report

Use:

Order_ID
Order_Date
Delivery_Date
Delivery_Days
Delivery_Status
Delivery_Performance

Create a final reporting query showing all six columns.

Sort by Delivery_Days in descending order.

Submission Requirements

For each task:

Load Sales_Data into Power Query.
Create a duplicate query or reference query for practice.
Use the appropriate Date, Time or Duration transformation.
Rename columns clearly.
Keep the original source columns unchanged wherever possible.
Apply transformations in the correct order.
Check the data type of each new column.
Load the final result back to Excel.
Keep each exercise as a separate query where appropriate.
Do not manually modify the source dataset.

Important Dataset Note:

The original Sales_Data dataset may contain only a Date column and may not contain Time, Delivery_Date, Delivery_Time or Duration columns.

For tasks requiring missing fields, create a separate practice query using Power Query's Enter Data feature or custom columns. Do not modify the original Sales_Data source.

Use proper data types:

Date → Date
Time → Time
DateTime → Date/Time
Duration → Duration
Year, Month, Day and Hour → Whole Number
Power Query Skills Covered

Date Transformations

Extract Year
Extract Month
Month Name
Extract Day
Day Name
Day of Week
Quarter of Year
Start of Month
End of Month
Start of Year
Week of Year

Date Calculations

Add Days
Subtract Days
Add Months
Add Years
Calculate Date Differences
Calculate Days Until Month End

Time Transformations

Extract Hour
Extract Minute
Extract Second
Start of Hour
Start of Minute
End of Hour
Time Classification

Duration Transformations

Days
Hours
Minutes
Seconds
Total Hours
Total Minutes
Total Seconds
Add Durations

Combined Skills

Date and Time Combination
DateTime Creation
Date Difference Calculation
Duration Calculation
Delivery Performance Analysis
Order Aging Analysis
Monthly Reporting
Quarterly Reporting
Business Calendar Creation
Conditional Columns
Business Reporting Preparation
