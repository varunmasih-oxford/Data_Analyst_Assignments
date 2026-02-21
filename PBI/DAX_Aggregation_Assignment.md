# DAX Aggregation Functions

Dataset Used: `DAX_Aggregation_Practice_Dataset.csv`

Columns:
OrderID, OrderDate, Quantity, UnitPrice, Discount, CustomerRating, Category, SalesRep, IsPriorityOrder

---

## 1. SUM

Use Case:
Calculate total numeric values in a column.

Example Scenario:
Find total quantity sold.

```DAX
Total Quantity = SUM(Sales[Quantity])
```

When to Use:
When you just need column aggregation without row-level calculation.

---

## 2. SUMX

Use Case:
Perform row-by-row calculation, then sum results.

Example Scenario:
Calculate total revenue.

```DAX
Total Revenue = SUMX(Sales, Sales[Quantity] * Sales[UnitPrice])
```

When to Use:
When calculation requires multiplying or combining columns per row.

---

## 3. AVERAGE

Use Case:
Calculate average of numeric column.

```DAX
Avg Price = AVERAGE(Sales[UnitPrice])
```

---

## 4. AVERAGEA

Use Case:
Average including logical values (TRUE = 1, FALSE = 0).

```DAX
Avg Priority = AVERAGEA(Sales[IsPriorityOrder])
```

---

## 5. AVERAGEX

Use Case:
Average of calculated expression.

```DAX
Avg Revenue = AVERAGEX(Sales, Sales[Quantity] * Sales[UnitPrice])
```

---

## 6. COUNT

Use Case:
Count numeric values (no blanks).

```DAX
Order Count = COUNT(Sales[OrderID])
```

---

## 7. COUNTA

Use Case:
Count non-blank values (text or numeric).

```DAX
Rating Count = COUNTA(Sales[CustomerRating])
```

---

## 8. COUNTROWS

Use Case:
Count number of rows in a table.

```DAX
Total Rows = COUNTROWS(Sales)
```

---

## 9. COUNTBLANK

Use Case:
Count blank values.

```DAX
Blank Discounts = COUNTBLANK(Sales[Discount])
```

---

## 10. COUNTX

Use Case:
Count rows where expression returns non-blank.

```DAX
Count Revenue Rows = COUNTX(Sales, Sales[Quantity] * Sales[UnitPrice])
```

---

## 11. COUNTAX

Use Case:
Like COUNTX but works with text/logical values.

```DAX
Count Text Example = COUNTAX(Sales, Sales[Category])
```

---

## 12. DISTINCTCOUNT

Use Case:
Count unique values.

```DAX
Unique Categories = DISTINCTCOUNT(Sales[Category])
```

---

## 13. DISTINCTCOUNTNOBLANK

Use Case:
Count unique values excluding blanks.

```DAX
Unique Ratings No Blank = DISTINCTCOUNTNOBLANK(Sales[CustomerRating])
```

---

## 14. MAX

Use Case:
Find highest numeric value.

```DAX
Max Price = MAX(Sales[UnitPrice])
```

---

## 15. MAXA

Use Case:
Works with logical values too.

```DAX
Max Priority = MAXA(Sales[IsPriorityOrder])
```

---

## 16. MAXX

Use Case:
Find maximum of expression.

```DAX
Max Revenue = MAXX(Sales, Sales[Quantity] * Sales[UnitPrice])
```

---

## 17. MIN

```DAX
Min Price = MIN(Sales[UnitPrice])
```

---

## 18. MINA

```DAX
Min Priority = MINA(Sales[IsPriorityOrder])
```

---

## 19. MINX

```DAX
Min Revenue = MINX(Sales, Sales[Quantity] * Sales[UnitPrice])
```

---

## 20. PRODUCT

Use Case:
Multiply all values in a column.

```DAX
Product Quantity = PRODUCT(Sales[Quantity])
```

---

## 21. PRODUCTX

Use Case:
Multiply expression row by row.

```DAX
Product Revenue = PRODUCTX(Sales, Sales[Quantity] * Sales[UnitPrice])
```

