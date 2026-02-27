# What-If Analysis in Excel — Complete Step-by-Step Learning Guide

---

## 1. Learning Objective

After completing this guide, you will be able to:

- Understand What-If Analysis
- Use Scenario Manager
- Use Goal Seek
- Create Data Tables
- Perform business decision analysis

---

## 2. Required Knowledge

Before starting:

- Basic Excel formulas
- Cell references
- SUM and multiplication formulas

---

## 3. Dataset (Used for All Examples)

Create the following dataset in Excel.

### Sales Dataset

| Cell | Field | Value |
|------|------|------|
| B2 | Product Price | 500 |
| B3 | Quantity Sold | 100 |
| B4 | Cost per Unit | 300 |

### Profit Calculation

| Cell | Field | Formula |
|------|------|---------|
| B6 | Revenue | =B2*B3 |
| B7 | Total Cost | =B4*B3 |
| B8 | Profit | =B6-B7 |

Inputs: Price, Quantity, Cost  
Output: Profit

---

## 4. Understanding What-If Analysis

What-If Analysis changes input values to observe how results change.

```

Input Values → Formula → Result
(Change Inputs) → New Result

```

---

## 5. Method 1 — Scenario Manager

Used to compare multiple business situations.

### Step 1: Open Scenario Manager

1. Go to Data tab
2. Click What-If Analysis
3. Select Scenario Manager

---

### Step 2: Create Best Case Scenario

Click Add.

Scenario Name: Best Case  
Changing Cells:
```

B2,B3,B4

```

Enter values:

| Price | Quantity | Cost |
|------|------|------|
| 600 | 150 | 280 |

Click OK.

---

### Step 3: Create Normal Case

| Price | Quantity | Cost |
|------|------|------|
| 500 | 100 | 300 |

---

### Step 4: Create Worst Case

| Price | Quantity | Cost |
|------|------|------|
| 450 | 70 | 320 |

---

### Step 5: View Scenario

Select scenario → Click Show.

Excel updates profit automatically.

---

### Learning Outcome

You compared multiple business conditions:

- Best case
- Normal case
- Worst case

---

## 6. Method 2 — Goal Seek

Goal Seek finds the required input to reach a target result.

### Business Problem

Target Profit = 50,000

---

### Steps

1. Go to Data tab
2. What-If Analysis
3. Click Goal Seek

Fill values:

| Option | Value |
|------|------|
| Set Cell | B8 |
| To Value | 50000 |
| By Changing Cell | B3 |

Click OK.

Excel calculates required quantity automatically.

---

### Learning Outcome

Goal Seek performs reverse calculation.

---

## 7. Method 3 — Data Table

Used to test many values at once.

---

### One-Variable Data Table

Question: What happens if price changes?

#### Step 1: Create Price List

| D2 | Price |
|----|------|
| D3 | 400 |
| D4 | 450 |
| D5 | 500 |
| D6 | 550 |
| D7 | 600 |

---

#### Step 2: Link Profit

In E2:
```

=B8

```

---

#### Step 3: Create Data Table

1. Select range D2:E7
2. Data → What-If Analysis → Data Table
3. Column Input Cell:
```

B2

```

Click OK.

Profit is calculated for all prices.

---

### Two-Variable Data Table

Question: What if Price and Quantity change?

#### Step 1: Setup Table

|   | 80 | 100 | 120 |
|---|---|---|---|
| 400 |   |   |   |
| 500 |   |   |   |
| 600 |   |   |   |

Top-left cell contains:
```

=B8

```

---

#### Step 2: Create Data Table

1. Select entire table
2. Data → What-If Analysis → Data Table

Input Cells:

| Input Type | Cell |
|------------|------|
| Row Input | B3 |
| Column Input | B2 |

Click OK.

Excel generates full profit comparison.

---

## 8. Real Business Use Cases

### Retail Store
Determine best selling price.

### Loan Analysis
Check EMI impact if interest changes.

### Sales Forecast
Identify required sales to achieve targets.

### Budget Planning
Analyze expenses vs profit.

---

## 9. Practice Exercises

### Exercise 1
Create a Data Table for quantities:
```

50, 75, 125, 200

```

---

### Exercise 2
Use Goal Seek:

Target Profit:
```

100000

```

Find required price.

---

### Exercise 3
Create scenarios:

- Festival Sale
- Discount Sale
- Low Demand

---

## 10. Recommended Learning Flow

1. Build formula model
2. Practice Goal Seek
3. Learn Scenario Manager
4. Practice Data Tables
5. Apply real business case study

---

## 11. Common Mistakes

- Selecting wrong input cells
- Missing formula reference
- Incorrect table selection
- Using text instead of numbers

---

## 12. Final Understanding

```

Change Inputs → Excel Recalculates → Better Decision Making

```
