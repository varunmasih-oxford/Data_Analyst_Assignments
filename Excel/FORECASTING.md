# FORECASTING IN EXCEL

## WHAT IS FORECASTING?

Forecasting in Excel is used to predict future values based on historical data. It helps identify trends and make data-driven decisions.

---

## EXAMPLE (SALES FORECASTING)

Imagine:

* You have past monthly sales data
* You want to predict future sales
* Excel uses patterns and trends to estimate upcoming values

---

## DATASET

| MONTH | SALES |
| ----- | ----- |
| Jan   | 200   |
| Feb   | 220   |
| Mar   | 250   |
| Apr   | 270   |
| May   | 300   |
| Jun   | 320   |

---

## METHODS FOR FORECASTING IN EXCEL

### 1. FORECAST FUNCTION

Formula:
`=FORECAST.LINEAR(x, known_y's, known_x's)`

Example:

* Predict sales for July (month 7):

`=FORECAST.LINEAR(7, B2:B7, A2:A7)`

---

### 2. FORECAST SHEET (EASIEST METHOD)

1. Select your data (Month and Sales)
2. Go to **Data → Forecast Sheet**
3. Choose chart type (Line or Column)
4. Set forecast end date
5. Click **Create**

Excel will generate:

* Forecast values
* Confidence intervals
* Chart visualization

---

### 3. TREND FUNCTION

Formula:
`=TREND(known_y's, known_x's, new_x's)`

Example:
`=TREND(B2:B7, A2:A7, A8)`

---

## STEP-BY-STEP (FORECAST SHEET)

1. Enter historical data
2. Select the dataset
3. Go to **Data → Forecast Sheet**
4. Adjust options (seasonality, timeline)
5. Click **Create**

---

## EXPECTED RESULT

Excel will:

* Predict future sales values
* Show trends in a chart
* Provide upper and lower confidence bounds

---

## COMMON USES

* Sales prediction
* Demand planning
* Financial forecasting
* Inventory management
* Trend analysis

---

## NOTES

* Data should be consistent (no gaps)
* Works best with time-based data
* More data improves accuracy

---
