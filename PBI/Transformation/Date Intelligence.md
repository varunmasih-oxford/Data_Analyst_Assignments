# Corporate Assignment: Date Intelligence in Power Query

## Scenario
You are working as a Data Analyst in a logistics company. The operations team is facing challenges in understanding shipment patterns, delivery timelines, and seasonal workload distribution.

Management wants a detailed time-based analysis using only date transformations to:
- Identify peak shipment periods
- Understand delivery cycles
- Improve planning and resource allocation

You are given raw shipment data and must transform it using date-based features.

---

## Dataset (CSV)

Save as: logistics_data.csv

```

Shipment_ID,Order_Date,Delivery_Date,Region,Shipment_Mode,Revenue
S001,08-02-2021,12-02-2021,North,Air,12000
S002,28-12-2020,04-01-2021,South,Road,8000
S003,15-03-2021,20-03-2021,East,Rail,6000
S004,01-01-2021,03-01-2021,West,Air,15000
S005,21-07-2021,30-07-2021,North,Road,9000
S006,11-11-2021,18-11-2021,South,Rail,7000
S007,05-05-2021,09-05-2021,East,Air,11000
S008,19-09-2021,25-09-2021,West,Road,5000
S009,30-06-2021,05-07-2021,North,Rail,4000
S010,14-02-2021,16-02-2021,South,Air,13000

```

---

## Objective
Use only Date Menu transformations in Power Query to extract insights and answer business questions.

---

## Tasks

### Task 1: Data Preparation
- Import the dataset
- Convert Order_Date and Delivery_Date to Date type
- Use parsing if required

---

### Task 2: Date Transformations

#### Year Level
Create the following from Order_Date:
- Year
- Start of Year
- End of Year
- Day of Year

#### Month Level
Create:
- Month Number
- Month Name
- Start of Month
- End of Month
- Days in Month

#### Quarter Level
Create:
- Quarter of Year
- Start of Quarter
- End of Quarter

#### Week Level
Create:
- Week of Year
- Week of Month
- Start of Week
- End of Week

#### Day Level
Create:
- Day
- Day of Week
- Name of Day

#### Additional
- Apply Age function on Order_Date
- Apply Date Only on Delivery_Date

---

## Scenario-Based Questions

### Section A: Business Understanding

1. The company wants to increase efficiency during high-demand periods.  
   - Identify which month has the highest number of shipments.
   - Suggest how operations can prepare for that period.

2. Management suspects uneven workload distribution across the year.  
   - Using quarter data, determine which quarter has the highest activity.
   - What business decisions can be made from this insight?

---

### Section B: Operational Analysis

3. The logistics head wants to optimize weekly planning.  
   - Identify the busiest week of the year.
   - How can this information improve workforce allocation?

4. There are complaints about delays on certain days.  
   - Analyze shipments by day name.
   - Which day has the highest shipment volume?

---

### Section C: Time Pattern Insights

5. The company wants to understand monthly shipment behavior.  
   - Compare shipments at the start vs end of the month.
   - What pattern do you observe?

6. Management is exploring seasonal trends.  
   - Use month and quarter data to identify any seasonal spikes.

---

### Section D: Strategic Thinking

7. The company is planning expansion.  
   - Based on yearly and quarterly trends, when should expansion be prioritized?

8. Weekend operations are under review.  
   - Using day-of-week analysis, determine if weekends are underutilized.

---

### Section E: Advanced Thinking

9. A manager wants to track shipment aging.  
   - Using the Age function, explain how old shipments can be monitored.

10. Why is it important to remove time values using Date Only in reporting?

---

## Expected Deliverables

- Transformed dataset with all date-based columns
- Dashboard including:
  - Monthly trend analysis
  - Quarterly comparison
  - Weekly shipment distribution
  - Day-wise performance

---
