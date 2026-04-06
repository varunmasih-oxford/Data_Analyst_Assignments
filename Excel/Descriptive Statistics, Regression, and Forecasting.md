# Retail Store Sales Forecasting Using Descriptive Statistics, Regression, and Forecasting

## Scenario
A retail store wants to understand how advertising spend affects sales and use that relationship to predict future sales.

---

## Step 1: Dataset

| Month | Ad Spend (₹1000) (X) | Sales (₹1000) (Y) |
|------|--------------------|------------------|
| Jan  | 10                 | 25               |
| Feb  | 15                 | 30               |
| Mar  | 20                 | 45               |
| Apr  | 25                 | 50               |
| May  | 30                 | 65               |
| Jun  | 35                 | 70               |

---

## Step 2: Descriptive Statistics (Understanding the Data)

### Mean Calculation
- Mean Ad Spend = (10+15+20+25+30+35)/6 = 22.5  
- Mean Sales = (25+30+45+50+65+70)/6 = 47.5  

### Range
- Sales range: 25 to 70  

### Relationship Insight
- As ad spend increases, sales also increase  
- Indicates a positive relationship  

### Conclusion from Descriptive Statistics
- Data shows an upward trend  
- No major outliers  
- Suitable for regression analysis  

---

## Step 3: Build Regression Model

Linear regression formula:

Y = a + bX

Where:
- Y = Sales  
- X = Ad Spend  
- a = Intercept  
- b = Slope  

### Calculated Values
- Slope (b) ≈ 1.8  
- Intercept (a) ≈ 7  

### Regression Equation
Y = 7 + 1.8X  

---

## Step 4: Model Interpretation

- Intercept (7): Base sales when ad spend is zero  
- Slope (1.8): For every increase of ₹1000 in ads, sales increase by ₹1800  

Conclusion:
Advertising has a strong positive impact on sales  

---

## Step 5: Forecasting Future Sales

Planned ad spend for next month: 40 (₹40,000)

Using regression equation:

Y = 7 + 1.8(40)  
Y = 7 + 72  
Y = 79  

Forecasted Sales = ₹79,000  

---

## Step 6: Final Understanding

- Descriptive statistics helped understand the data  
- Regression created a mathematical relationship  
- Forecasting predicted future outcomes  

---

## Step 7: Why This Approach Works

- Data follows a clear linear trend  
- Variables are strongly related  
- No extreme variations  

---

## Step 8: Business Application

- Helps in planning marketing budgets  
- Allows prediction of revenue  
- Supports better decision-making  

---
