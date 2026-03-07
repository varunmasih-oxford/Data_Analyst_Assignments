# Power BI Data Cleaning and Transformation
## Dataset

File: powerbi_messy_sales_dataset.csv

------------------------------------------------------------------------

# Problem Statement

You are working as a Data Analyst in an electronics retail company. The
company collected sales data from different branches, but the dataset
contains multiple quality issues due to manual entry and inconsistent
systems.

Your task is to clean and transform the dataset using Power BI Power
Query Editor so that it becomes usable for analysis and reporting.

After cleaning the data, the company wants to analyze:

-   Total sales revenue
-   Sales by city
-   Product performance
-   Monthly sales trends
-   Impact of discount on sales

------------------------------------------------------------------------

# Dataset Columns

  Column         Description
  -------------- ------------------------------------
  OrderID        Order number (contains duplicates)
  CustomerName   Name of the customer
  City           Customer city
  Product        Product purchased
  Category       Product category
  OrderDate      Date of order
  Quantity       Number of units purchased
  Price          Product price
  Discount%      Discount given

------------------------------------------------------------------------

# Problems Present in the Dataset

## Duplicate Records

Some OrderID values appear multiple times.

Example: OrderID\
1015\
1015

------------------------------------------------------------------------

## Missing Values

Some columns contain null values:

-   City
-   Quantity
-   Price
-   OrderDate
-   Discount%

------------------------------------------------------------------------

## Inconsistent Date Formats

Dates appear in different formats such as:

2024-03-10\
15/02/2024\
03-25-2024

These must be converted into a standard Date format.

------------------------------------------------------------------------

## Price Column Contains Text

Price values appear as:

5000\
₹4500\
6000 INR

Currency symbols and text must be removed.

------------------------------------------------------------------------

## City Column Inconsistencies

City names contain:

Delhi\
delhi\
Delhi

Issues include:

-   Lowercase values
-   Extra spaces
-   Inconsistent formatting

------------------------------------------------------------------------

## Quantity Data Type Issues

Quantity values appear as:

5\
"7"\
NULL

These must be converted to Whole Number.

------------------------------------------------------------------------

## Discount Column Contains Null Values

Some rows have missing discount values.

------------------------------------------------------------------------

# Power BI Transformation Steps

## Step 1 Import Dataset

1.  Open Power BI Desktop
2.  Click Get Data
3.  Choose Text/CSV
4.  Select the dataset
5.  Click Transform Data

This will open the Power Query Editor.

------------------------------------------------------------------------

# Step 2 Remove Duplicate Orders

1.  Select the OrderID column
2.  Go to Home tab
3.  Click Remove Rows
4.  Click Remove Duplicates

------------------------------------------------------------------------

# Step 3 Clean City Column

Select the City column.

Apply the following:

Transform → Format → Trim\
Transform → Format → Clean

Then convert to proper format:

Transform → Format → Capitalize Each Word

Example:

delhi → Delhi\
Delhi → Delhi

------------------------------------------------------------------------

# Step 4 Handle Missing City Values

1.  Select City column
2.  Go to Transform
3.  Click Replace Values
4.  Replace null with Unknown

------------------------------------------------------------------------

# Step 5 Clean Price Column

Remove currency symbols.

1.  Select Price column
2.  Go to Transform
3.  Click Replace Values

Replace:

₹ → blank\
INR → blank

Then change datatype:

Transform → Data Type → Whole Number

------------------------------------------------------------------------

# Step 6 Fix Quantity Column

1.  Select Quantity column
2.  Transform → Data Type → Whole Number

Replace null values with 1.

------------------------------------------------------------------------

# Step 7 Fix Order Date Column

1.  Select OrderDate column
2.  Transform → Data Type → Date

If errors appear:

Transform → Detect Data Type

Or use:

Using Locale → Date → English (India)

------------------------------------------------------------------------

# Step 8 Handle Discount Null Values

1.  Select Discount% column
2.  Replace null values with 0

------------------------------------------------------------------------

# Step 9 Create Total Sales Column

Go to:

Add Column → Custom Column

Formula:

TotalSales = \[Quantity\] \* \[Price\] \* (1 - \[Discount%\]/100)

------------------------------------------------------------------------

# Step 10 Extract Year and Month

Select OrderDate column.

Add:

Add Column → Date → Year\
Add Column → Date → Month

------------------------------------------------------------------------

# Final Clean Dataset Should Contain

OrderID\
CustomerName\
City\
Product\
Category\
OrderDate\
Year\
Month\
Quantity\
Price\
Discount%\
TotalSales

------------------------------------------------------------------------

# Analysis Tasks

Create the following visuals in Power BI:

1.  Total Sales Card
2.  Sales by City (Bar Chart)
3.  Sales by Product (Column Chart)
4.  Monthly Sales Trend (Line Chart)
5.  Sales by Category (Pie Chart)
6.  Top 5 Products by Sales

------------------------------------------------------------------------

# Advanced Practice

## Create Profit Column

Profit = TotalSales \* 0.25

------------------------------------------------------------------------

## Average Order Value

Average Order Value = TotalSales / Quantity

------------------------------------------------------------------------

## Product Ranking

Rank products based on Total Sales.
