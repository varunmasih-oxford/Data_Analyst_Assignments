# Project 2: HR & Employee Analytics

## 1. Business Scenario

The HR leadership team wants to understand workforce performance, employee satisfaction, attendance, training effectiveness and attrition across departments and offices.

Your task is to act as a **Business Data Analyst** and convert the raw operational data into a Pivot Table-based management report.

---

## 2. Dataset Overview

This project is designed to practice:

- Excel Tables
- Pivot Tables
- Pivot Charts
- Slicers
- Timeline
- KPI calculations
- Benchmark comparison
- Conditional Formatting
- Business insights
- Management decision-making

### Dataset Columns

| Column | Description |
|---|---|
| Employee_ID | Unique employee identifier |
| Month | Reporting month |
| Department | Employee department |
| Location | Office location |
| Job_Level | Job level |
| Employment_Type | Full-time / Part-time |
| Gender | Employee gender |
| Age_Group | Age category |
| Experience_Years | Years of experience |
| Salary | Monthly salary |
| Attendance_% | Attendance percentage |
| Training_Hours | Training hours |
| Performance_Score | Performance score out of 100 |
| Overtime_Hours | Monthly overtime hours |
| Satisfaction_Score | Employee satisfaction out of 5 |
| Attrition | Yes/No |
| Absence_Days | Absence days |

---

## 3. Dataset

Save the following data as:

`02_hr_employee_analytics.csv`

```csv
Employee_ID,Month,Department,Location,Job_Level,Employment_Type,Gender,Age_Group,Experience_Years,Salary,Attendance_%,Training_Hours,Performance_Score,Overtime_Hours,Satisfaction_Score,Attrition,Absence_Days
EMP001,2026-01,Marketing,Delhi,Junior,Part-time,Male,26-30,2,31358,94.5,2,66.0,6,3.5,Yes,4
EMP002,2026-02,Finance,Bangalore,Senior,Part-time,Male,31-40,10,80189,98.5,7,68.4,12,3.2,Yes,6
EMP003,2026-03,Marketing,Mumbai,Junior,Part-time,Female,21-25,3,39850,88.8,12,72.5,9,5.0,No,6
EMP004,2026-04,Finance,Noida,Mid,Part-time,Male,26-30,4,64960,96.0,4,80.3,8,5.0,No,5
EMP005,2026-05,IT,Delhi,Senior,Part-time,Female,31-40,5,102717,97.7,12,80.1,8,3.3,No,5
EMP006,2026-06,HR,Gurgaon,Mid,Full-time,Male,51+,2,65560,95.5,11,67.1,12,4.2,No,3
EMP007,2026-01,Marketing,Bangalore,Senior,Full-time,Male,31-40,7,70212,97.6,6,97.1,24,3.4,No,0
EMP008,2026-02,HR,Gurgaon,Junior,Full-time,Male,51+,2,39894,88.6,16,83.7,2,3.2,No,3
EMP009,2026-03,Marketing,Mumbai,Mid,Full-time,Female,26-30,6,62671,91.4,12,86.4,14,4.8,No,3
EMP010,2026-04,Sales,Bangalore,Mid,Part-time,Male,51+,2,47208,91.6,10,72.9,21,4.0,No,4
EMP011,2026-05,Finance,Mumbai,Mid,Full-time,Male,21-25,2,58879,97.5,2,87.2,20,3.2,No,3
EMP012,2026-06,IT,Bangalore,Manager,Full-time,Male,21-25,12,129041,96.9,15,83.2,1,4.3,No,4
EMP013,2026-01,Finance,Mumbai,Manager,Part-time,Male,51+,10,117380,98.2,14,80.0,13,4.4,No,5
EMP014,2026-02,IT,Noida,Mid,Full-time,Male,26-30,6,46873,93.2,16,93.1,5,3.1,No,4
EMP015,2026-03,Marketing,Gurgaon,Manager,Part-time,Female,26-30,8,137042,93.8,16,73.6,21,4.4,No,1
EMP016,2026-04,HR,Delhi,Junior,Part-time,Male,41-50,3,30400,90.9,16,76.5,2,4.8,No,2
EMP017,2026-05,Marketing,Bangalore,Senior,Part-time,Female,31-40,7,106256,91.0,11,72.0,10,3.4,Yes,5
EMP018,2026-06,Sales,Delhi,Manager,Full-time,Female,26-30,13,110589,96.2,10,88.3,17,3.0,No,0
EMP019,2026-01,Operations,Bangalore,Mid,Full-time,Male,41-50,3,74457,91.9,12,73.2,3,3.7,No,4
EMP020,2026-02,IT,Gurgaon,Manager,Full-time,Female,26-30,13,117485,89.8,13,68.6,27,3.1,Yes,3
EMP021,2026-03,HR,Noida,Mid,Part-time,Male,51+,2,55756,88.8,14,74.2,20,4.0,No,5
EMP022,2026-04,Sales,Noida,Mid,Full-time,Male,41-50,2,68872,94.7,10,68.8,28,4.2,Yes,2
EMP023,2026-05,HR,Mumbai,Junior,Full-time,Female,41-50,2,37840,92.5,8,88.0,17,3.3,No,3
EMP024,2026-06,Finance,Bangalore,Junior,Part-time,Female,21-25,2,38559,95.4,10,80.6,28,4.9,No,5
EMP025,2026-01,Sales,Gurgaon,Senior,Part-time,Female,41-50,6,101138,97.3,3,80.0,28,4.3,No,1
EMP026,2026-02,IT,Gurgaon,Junior,Part-time,Female,51+,0,44972,90.7,15,69.0,4,4.6,No,5
EMP027,2026-03,Operations,Bangalore,Manager,Full-time,Female,31-40,15,155041,95.0,14,90.7,15,4.3,No,2
EMP028,2026-04,HR,Noida,Junior,Full-time,Female,51+,1,33007,92.6,7,82.9,13,3.1,No,6
EMP029,2026-05,Finance,Delhi,Senior,Full-time,Male,41-50,8,87887,93.3,8,76.1,21,4.6,No,5
EMP030,2026-06,Finance,Bangalore,Junior,Part-time,Male,41-50,0,33954,91.6,9,75.8,24,4.8,No,2
EMP031,2026-01,Finance,Delhi,Junior,Part-time,Female,26-30,2,29319,90.2,2,85.5,7,3.3,No,5
EMP032,2026-02,HR,Gurgaon,Junior,Full-time,Male,31-40,1,38222,98.4,5,67.5,22,4.7,No,1
EMP033,2026-03,HR,Bangalore,Manager,Full-time,Female,41-50,13,153892,93.4,8,96.7,20,4.8,No,3
EMP034,2026-04,Operations,Bangalore,Manager,Part-time,Male,41-50,12,154442,98.3,6,94.1,7,4.5,No,4
EMP035,2026-05,Finance,Noida,Mid,Part-time,Male,41-50,3,54163,97.7,10,65.3,30,3.4,Yes,1
EMP036,2026-06,Marketing,Mumbai,Manager,Part-time,Female,31-40,12,120067,95.3,7,80.6,16,3.7,No,5
EMP037,2026-01,HR,Noida,Mid,Part-time,Male,26-30,3,51276,93.3,13,84.5,24,4.0,No,2
EMP038,2026-02,HR,Gurgaon,Senior,Part-time,Female,31-40,6,106264,95.7,4,86.0,24,4.0,Yes,6
EMP039,2026-03,Finance,Noida,Mid,Full-time,Female,26-30,4,58130,94.3,12,66.8,4,4.6,No,2
EMP040,2026-04,Operations,Bangalore,Mid,Full-time,Male,31-40,5,55006,88.7,13,68.3,24,3.4,Yes,1
EMP041,2026-05,IT,Gurgaon,Junior,Full-time,Female,51+,1,43398,91.2,6,88.2,14,3.1,No,1
EMP042,2026-06,Sales,Bangalore,Mid,Part-time,Female,41-50,4,50436,96.2,11,95.4,14,3.2,No,5
EMP043,2026-01,Finance,Delhi,Junior,Full-time,Male,51+,3,28847,97.2,11,84.4,0,5.0,No,5
EMP044,2026-02,Finance,Bangalore,Manager,Part-time,Male,31-40,14,122803,92.5,7,87.1,27,3.3,No,3
EMP045,2026-03,Finance,Delhi,Senior,Full-time,Male,41-50,5,70075,97.6,9,78.6,6,4.0,No,4
EMP046,2026-04,HR,Bangalore,Mid,Part-time,Male,21-25,5,45945,90.6,4,75.3,0,4.1,No,0
EMP047,2026-05,Marketing,Gurgaon,Manager,Full-time,Female,26-30,12,130947,90.7,10,69.8,6,4.8,No,4
EMP048,2026-06,Finance,Noida,Senior,Full-time,Female,26-30,10,79738,93.9,7,76.0,24,4.1,No,3
EMP049,2026-01,IT,Mumbai,Junior,Full-time,Female,41-50,2,40651,98.6,4,81.6,18,3.7,No,0
EMP050,2026-02,Sales,Gurgaon,Manager,Full-time,Male,41-50,12,142587,88.9,7,93.1,27,4.1,No,2
EMP051,2026-03,IT,Noida,Mid,Part-time,Male,51+,5,50451,88.3,7,91.3,9,3.7,No,3
EMP052,2026-04,IT,Gurgaon,Junior,Full-time,Male,31-40,3,44307,90.6,12,73.4,8,4.3,No,6
EMP053,2026-05,Finance,Noida,Senior,Part-time,Male,41-50,8,101667,90.6,11,76.8,9,5.0,Yes,2
EMP054,2026-06,Operations,Delhi,Manager,Part-time,Female,21-25,13,140690,90.8,14,88.8,21,4.4,No,1
EMP055,2026-01,Sales,Bangalore,Senior,Part-time,Female,31-40,7,83159,96.7,16,97.1,16,4.0,No,2
EMP056,2026-02,Marketing,Noida,Junior,Part-time,Female,31-40,3,41022,89.0,8,65.5,17,3.2,Yes,2
EMP057,2026-03,Sales,Gurgaon,Manager,Part-time,Female,21-25,13,141641,97.1,16,88.1,20,3.8,Yes,1
EMP058,2026-04,Sales,Delhi,Mid,Full-time,Female,31-40,5,64245,92.6,3,92.5,19,3.8,Yes,2
EMP059,2026-05,Finance,Gurgaon,Senior,Full-time,Female,21-25,9,88080,98.7,15,92.2,2,4.3,No,5
EMP060,2026-06,IT,Gurgaon,Mid,Full-time,Male,26-30,6,55766,97.9,2,74.2,4,5.0,No,4
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| Attendance | 95% or higher |
| Performance Score | 80 or higher |
| Satisfaction | 4.0 or higher |
| Attrition Rate | 10% or lower |
| Training Hours | 8+ per month |
| Absence Days | 3 or fewer |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **Attrition Rate**: `Attrition Yes employees / Total Employees × 100`
- **Average Salary**: `Total Salary / Employee Count`
- **Average Performance**: `Average Performance Score`
- **Average Satisfaction**: `Average Satisfaction Score`
- **Training per Employee**: `Total Training Hours / Employee Count`

---

## 6. Assignment Tasks

### Task 1 — Department Performance
Create a Pivot Table with **Department** as Rows and Average Salary, Average Attendance, Average Performance Score, Average Satisfaction, Average Training Hours and Count of Employees as Values. Identify the strongest department.
### Task 2 — Attrition Analysis
Create a Pivot Table by Department and Attrition. Show employee count and calculate attrition rate. Compare each department with the 10% benchmark.
### Task 3 — Job-Level Analysis
Compare Junior, Mid, Senior and Manager employees using salary, performance, satisfaction, training and overtime.
### Task 4 — Location Analysis
Compare offices by headcount, salary, attendance, performance and attrition.
### Task 5 — Performance vs Satisfaction
Create a Pivot Table using Performance Score and Satisfaction Score by Department. Identify departments where performance is high but satisfaction is low.
### Task 6 — Monthly HR Trend
Group Month and analyze headcount, average attendance, performance, overtime and attrition.
### Task 7 — Training Effectiveness
Compare employees with lower vs higher Training Hours and analyze their average Performance Score and Satisfaction Score.
### Task 8 — Employee Benchmark Status
Create benchmark status columns for attendance, performance, satisfaction and absence.
### Task 9 — HR Dashboard
Create KPI cards, Pivot Charts, slicers for Department, Location, Job Level and Attrition, plus a monthly timeline.
### Task 10 — Management Recommendations
Identify the top three HR issues and propose practical actions.

---

## 7. Recommended Pivot Charts

1. **Headcount by Department** — Column Chart
2. **Attrition Rate by Department** — Bar Chart
3. **Average Performance by Job Level** — Column Chart
4. **Monthly Attrition Trend** — Line Chart
5. **Salary by Department** — Bar Chart
6. **Attendance vs Performance** — Scatter Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Total Employees
- Average Salary
- Average Performance
- Average Satisfaction
- Attendance %
- Attrition Rate
- Training Hours
- Average Overtime

### Filters / Slicers

- Department
- Location
- Job_Level
- Employment_Type
- Attrition

### Dashboard Charts

- Headcount by Department
- Attrition Rate by Department
- Performance by Job Level
- Monthly Attrition Trend

---

## 9. Final Business Questions

1. Which department has the highest headcount?
2. Which department has the highest attrition rate?
3. Which department has the best performance?
4. Which location performs best?
5. Does more training appear associated with better performance?
6. Which job level has the highest average salary?
7. Which department is below the satisfaction benchmark?
8. Which HR KPI needs immediate attention?
9. What three retention actions should management take?

---

## 10. Final Management Challenge

Management wants to reduce avoidable attrition without reducing productivity. Use your Pivot Tables to identify the department, employee group and KPI that deserve priority.

---

## 11. Final Deliverable

Create an Excel workbook with:

1. **Raw Data**
2. **Analysis / Pivot Tables**
3. **KPI / Benchmark Analysis**
4. **Charts**
5. **Dashboard**
6. **Management Recommendations**

### Expected Workflow

```text
Raw Data
   ↓
Excel Table
   ↓
Pivot Tables
   ↓
Calculated KPIs
   ↓
Benchmark Comparison
   ↓
Pivot Charts
   ↓
Slicers / Timeline
   ↓
Dashboard
   ↓
Business Insights
   ↓
Management Decisions
```
