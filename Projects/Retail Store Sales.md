# Project: Retail Store Sales Data Analysis Using Python

## 1. Project Objective

Analyze retail sales data to:

* Identify top-selling products
* Analyze monthly revenue trends
* Compare city-wise performance
* Evaluate category contribution
* Generate business insights

This project uses:

* NumPy (numerical operations)
* Pandas (data manipulation)
* Matplotlib (data visualization)

---

# 2. Project Folder Structure

```
sales_analysis_project/
│
├── dataset/
│   └── sales_data.csv
│
├── analysis.py
└── README.md
```

---

# 3. Dataset Structure (sales_data.csv)

Columns:

* Order_ID
* Order_Date
* Customer_Name
* City
* Product
* Category
* Quantity
* Unit_Price
* Total_Sales

### Sample Data (First 10 Rows)

```
Order_ID,Order_Date,Customer_Name,City,Product,Category,Quantity,Unit_Price,Total_Sales
1001,2025-01-05,Rahul Sharma,Delhi,Laptop,Electronics,1,55000,55000
1002,2025-01-06,Anita Verma,Mumbai,Smartphone,Electronics,2,20000,40000
1003,2025-01-07,Rohit Kumar,Bangalore,Office Chair,Furniture,3,5000,15000
1004,2025-01-08,Priya Singh,Delhi,Tablet,Electronics,1,30000,30000
1005,2025-01-09,Amit Shah,Chennai,Desk,Furniture,2,8000,16000
1006,2025-01-10,Neha Jain,Kolkata,Headphones,Accessories,4,2000,8000
1007,2025-01-11,Vikas Mehta,Mumbai,Monitor,Electronics,2,12000,24000
1008,2025-01-12,Sneha Roy,Delhi,Keyboard,Accessories,5,1500,7500
1009,2025-01-13,Arjun Nair,Bangalore,Mouse,Accessories,6,1000,6000
1010,2025-01-14,Kiran Patel,Chennai,Printer,Electronics,1,15000,15000
```

Expand this to 100 rows for a realistic project.

---

# 4. Step-by-Step Implementation (analysis.py)

## Step 1: Import Libraries

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

---

## Step 2: Load Dataset

```python
df = pd.read_csv("dataset/sales_data.csv")

print("First 5 Rows:")
print(df.head())

print("\nDataset Info:")
print(df.info())
```

---

## Step 3: Data Cleaning

```python
# Check missing values
print(df.isnull().sum())

# Convert Order_Date to datetime
df['Order_Date'] = pd.to_datetime(df['Order_Date'])

# Create Month column
df['Month'] = df['Order_Date'].dt.month
```

---

# 5. Data Analysis Using Pandas and NumPy

## Total Revenue

```python
total_revenue = np.sum(df['Total_Sales'])
print("Total Revenue:", total_revenue)
```

---

## City-wise Sales

```python
city_sales = df.groupby("City")["Total_Sales"].sum()
print(city_sales)
```

---

## Product-wise Sales

```python
product_sales = df.groupby("Product")["Total_Sales"].sum()
print(product_sales.sort_values(ascending=False))
```

---

## Monthly Sales Trend

```python
monthly_sales = df.groupby("Month")["Total_Sales"].sum()
print(monthly_sales)
```

---

# 6. Data Visualization Using Matplotlib

## City Wise Sales (Bar Chart)

```python
plt.figure()
city_sales.plot(kind="bar")
plt.title("City Wise Sales")
plt.xlabel("City")
plt.ylabel("Total Sales")
plt.show()
```

---

## Monthly Sales Trend (Line Chart)

```python
plt.figure()
monthly_sales.plot()
plt.title("Monthly Sales Trend")
plt.xlabel("Month")
plt.ylabel("Revenue")
plt.show()
```

---

## Category Contribution (Pie Chart)

```python
category_sales = df.groupby("Category")["Total_Sales"].sum()

plt.figure()
plt.pie(category_sales, labels=category_sales.index, autopct="%1.1f%%")
plt.title("Category Contribution")
plt.show()
```

---

## Top 5 Products

```python
top_products = product_sales.sort_values(ascending=False).head(5)

plt.figure()
top_products.plot(kind="bar")
plt.title("Top 5 Selling Products")
plt.xlabel("Product")
plt.ylabel("Sales")
plt.show()
```

---

# 7. Advanced Analysis

## Average Order Value

```python
avg_order = df['Total_Sales'].mean()
print("Average Order Value:", avg_order)
```

---

## Highest Single Order

```python
highest_order = df.loc[df['Total_Sales'].idxmax()]
print(highest_order)
```

---

## Sales Standard Deviation

```python
std_sales = np.std(df['Total_Sales'])
print("Sales Standard Deviation:", std_sales)
```

---

# 8. Business Insights (Important for Interview)

After running the project, explain:

* Which city generates the highest revenue
* Which category contributes most
* Which month has peak sales
* Top performing products
* Whether sales are consistent or highly variable

Interviewers focus more on insights than code.

---

