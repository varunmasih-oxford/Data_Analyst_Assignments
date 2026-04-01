# SOLVER IN EXCEL

## WHAT IS SOLVER?

Solver is a tool in Microsoft Excel used for optimization. It helps you find the best value (maximum, minimum, or a specific target) for a formula by changing selected input cells, subject to constraints.

---
## Example (Simple Understanding)

Imagine:

* You want to maximize profit
* Profit depends on number of units produced
* But you have limits (budget, materials)

Solver finds the best numbers automatically.

---
## How to Use Solver (Step-by-Step)

### 1. Set up your sheet:

* Objective cell → the result (e.g., profit)
* Variable cells → values Solver can change
* Constraints → limits (e.g., ≤ budget)

### 2. Open Solver:

* Go to Data → Solver

### 3. Fill in:

* Set Objective → select result cell

Choose:

* Max

* Min

* Value Of

* By Changing Variable Cells → select input cells

### 4. Add Constraints:

* Click Add

Example:

* A1 ≤ 100
* B1 ≥ 0

### 5. Click Solve

---

## Common Uses

* Budget planning
* Production optimization
* Scheduling
* Resource allocation
* Portfolio optimization


## HOW TO ENABLE SOLVER

1. Open Excel
2. Go to **File → Options → Add-ins**
3. At the bottom, select **Excel Add-ins → Go**
4. Check **Solver Add-in**
5. Click **OK**

Solver will now appear in the **Data** tab.

---

## EXAMPLE: MAXIMIZING PROFIT

### PROBLEM STATEMENT

A company produces two products: Product A and Product B. Each product requires labor and material. The goal is to maximize profit given limited resources.

---

## DATASET

| ITEM                | PRODUCT A | PRODUCT B | AVAILABLE |
| ------------------- | --------- | --------- | --------- |
| PROFIT PER UNIT     | 20        | 30        |           |
| LABOR HOURS/UNIT    | 2         | 1         | 100       |
| MATERIAL UNITS/UNIT | 1         | 2         | 80        |
| UNITS TO PRODUCE    | (A)       | (B)       |           |

---

## EXCEL SETUP

1. Enter the dataset in Excel

2. Let:

   * Cell B5 = Units of Product A
   * Cell C5 = Units of Product B

3. Create formulas:

* TOTAL PROFIT (OBJECTIVE CELL):
  `=20*B5 + 30*C5`

* LABOR USED:
  `=2*B5 + 1*C5`

* MATERIAL USED:
  `=1*B5 + 2*C5`

---

## SOLVER CONFIGURATION

1. Go to **Data → Solver**

2. Set parameters:

* SET OBJECTIVE: Total Profit cell

* Select **MAX**

* BY CHANGING VARIABLE CELLS:
  B5, C5

3. Add constraints:

* Labor Used ≤ 100
* Material Used ≤ 80
* B5 ≥ 0
* C5 ≥ 0

4. Choose solving method:

* SIMPLEX LP

5. Click **SOLVE**

---

## EXPECTED RESULT

Solver will give optimal values for:

* Product A = 40 units
* Product B = 20 units
* Maximum Profit = 1400

---

## NOTES

* Ensure formulas are correct before running Solver
* Use Simplex LP for linear problems
* Add integer constraints if only whole units are allowed

---
