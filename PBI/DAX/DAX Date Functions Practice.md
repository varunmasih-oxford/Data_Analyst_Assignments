# DAX Date Functions Practice

## Dataset Columns

* Order ID
* Order Date
* Ship Date
* Segment
* Ship Mode

---

## 1. Extract Date Parts

### Use Case

Analyze orders by year, month, or day.

### Calculated Columns

```DAX
Order Year = YEAR('Orders'[Order Date])

Order Month = FORMAT('Orders'[Order Date], "MMMM")

Order Month No = MONTH('Orders'[Order Date])

Order Day = DAY('Orders'[Order Date])
```

### Outcome

Helps build visuals like:

* Orders by Month
* Orders by Year

---

## 2. Shipping Delay

### Use Case

Calculate how many days it takes to ship an order.

### Calculated Column

```DAX
Shipping Days = DATEDIFF('Orders'[Order Date], 'Orders'[Ship Date], DAY)
```

### Outcome

* Identify slow deliveries
* Compare shipping performance

---

## 3. Delivery Status Classification

### Use Case

Classify orders based on delivery speed.

### Calculated Column

```DAX
Delivery Status = 
IF(
    'Orders'[Shipping Days] <= 2, "Fast",
    IF('Orders'[Shipping Days] <= 5, "Normal", "Delayed")
)
```

### Outcome

Used for KPI tracking and filtering delayed orders.

---

## 4. Orders This Month

### Use Case

Track current month order count.

### Measure

```DAX
Orders This Month = 
CALCULATE(
    COUNT('Orders'[Order ID]),
    MONTH('Orders'[Order Date]) = MONTH(TODAY()) &&
    YEAR('Orders'[Order Date]) = YEAR(TODAY())
)
```

---

## 5. Orders in Last 30 Days

### Use Case

Rolling time-based analysis.

### Measure

```DAX
Orders Last 30 Days =
CALCULATE(
    COUNT('Orders'[Order ID]),
    'Orders'[Order Date] >= TODAY() - 30
)
```

---

## 6. Weekday vs Weekend Orders

### Use Case

Understand order patterns.

### Calculated Column

```DAX
Day Type = 
IF(
    WEEKDAY('Orders'[Order Date], 2) > 5,
    "Weekend",
    "Weekday"
)
```

---

## 7. Orders Same Period Last Year

### Use Case

Year-over-year comparison.

### Measure

```DAX
Orders Last Year =
CALCULATE(
    COUNT('Orders'[Order ID]),
    SAMEPERIODLASTYEAR('Orders'[Order Date])
)
```

---

## 8. Month-Year Format

### Use Case

Improve readability in reports.

### Calculated Column

```DAX
Month Year = FORMAT('Orders'[Order Date], "MMM YYYY")
```

---

## 9. Late Shipment Indicator

### Use Case

Identify delayed shipments.

### Calculated Column

```DAX
Late Shipment = 
IF('Orders'[Shipping Days] > 5, "Yes", "No")
```

---

## 10. Average Shipping Days

### Use Case

Measure delivery efficiency.

### Measure

```DAX
Avg Shipping Days = 
AVERAGE('Orders'[Shipping Days])
```

