# Project 6: Education / Institute Analytics

## 1. Business Scenario

A training institute wants to analyze admissions, fees, attendance, academic performance, student satisfaction, completion and placement outcomes.

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
| Student_ID | Student identifier |
| Month | Admission month |
| Course | Course enrolled |
| Batch | Batch name |
| Trainer | Trainer |
| Lead_Source | Lead source |
| Student_Type | New/Returning |
| Course_Fee | Course fee |
| Paid_Amount | Amount paid |
| Attendance_% | Attendance percentage |
| Test_Score | Average test score |
| Assignments_Completed_% | Assignment completion |
| Satisfaction | Student satisfaction out of 5 |
| Completion_Status | Completed/Ongoing/Dropped |
| Placement_Status | Placed/Not Placed/NA |

---

## 3. Dataset

Save the following data as:

`06_education_institute_analytics.csv`

```csv
Student_ID,Month,Course,Batch,Trainer,Lead_Source,Student_Type,Course_Fee,Paid_Amount,Attendance_%,Test_Score,Assignments_Completed_%,Satisfaction,Completion_Status,Placement_Status
STU001,2026-01,Advanced Excel,Batch-6,Trainer A,Instagram,New,30000,30000,80.4,76.5,82.7,3.9,Completed,Placed
STU002,2026-02,Data Analytics,Batch-5,Trainer D,Instagram,Returning,15000,6201,77.1,75.3,75.3,3.5,Ongoing,NA
STU003,2026-03,Data Analytics,Batch-2,Trainer B,WhatsApp,New,20000,20000,90.9,66.7,63.1,3.9,Completed,Not Placed
STU004,2026-04,Data Analytics,Batch-3,Trainer B,Referral,Returning,30000,30000,83.5,67.1,93.8,3.8,Completed,Not Placed
STU005,2026-05,Python Programming,Batch-2,Trainer A,Walk-in,New,50000,50000,83.5,80.4,79.7,4.6,Completed,Not Placed
STU006,2026-06,Digital Marketing,Batch-6,Trainer C,Google,New,20000,20000,88.4,84.8,60.4,3.8,Ongoing,NA
STU007,2026-01,Data Analytics,Batch-1,Trainer B,WhatsApp,Returning,40000,29756,84.3,57.6,99.9,4.5,Ongoing,NA
STU008,2026-02,Digital Marketing,Batch-1,Trainer A,Walk-in,New,50000,35022,98.3,58.7,63.8,3.4,Ongoing,NA
STU009,2026-03,Python Programming,Batch-1,Trainer B,Instagram,New,20000,20000,94.7,94.8,75.7,4.7,Completed,Placed
STU010,2026-04,Digital Marketing,Batch-3,Trainer D,Referral,New,20000,20000,83.0,68.5,64.8,3.8,Ongoing,NA
STU011,2026-05,Web Development,Batch-2,Trainer A,Instagram,Returning,15000,15000,89.9,90.5,87.9,3.3,Ongoing,NA
STU012,2026-06,Digital Marketing,Batch-5,Trainer B,Google,Returning,30000,30000,89.6,66.2,99.6,3.3,Completed,Not Placed
STU013,2026-01,Digital Marketing,Batch-3,Trainer A,WhatsApp,Returning,15000,8290,73.5,57.7,91.2,3.6,Dropped,NA
STU014,2026-02,Web Development,Batch-1,Trainer A,Walk-in,New,15000,15000,71.9,93.8,77.7,3.4,Ongoing,NA
STU015,2026-03,Python Programming,Batch-2,Trainer C,Referral,Returning,20000,15096,93.8,72.0,61.2,4.4,Completed,Not Placed
STU016,2026-04,Data Analytics,Batch-1,Trainer C,Walk-in,New,20000,20000,88.0,65.6,71.8,3.9,Completed,Not Placed
STU017,2026-05,Digital Marketing,Batch-6,Trainer C,Walk-in,Returning,30000,30000,95.7,77.6,85.2,4.6,Ongoing,NA
STU018,2026-06,Data Analytics,Batch-3,Trainer A,Walk-in,Returning,25000,18231,79.3,66.6,61.0,4.3,Ongoing,NA
STU019,2026-01,Data Analytics,Batch-2,Trainer D,Referral,New,40000,21230,72.9,83.2,70.7,4.7,Ongoing,NA
STU020,2026-02,AI & Machine Learning,Batch-6,Trainer C,WhatsApp,New,20000,20000,79.2,86.7,74.4,4.3,Ongoing,NA
STU021,2026-03,Data Analytics,Batch-5,Trainer D,Google,Returning,40000,32129,85.7,62.5,61.5,3.3,Completed,Not Placed
STU022,2026-04,Data Analytics,Batch-2,Trainer B,Google,Returning,40000,40000,73.8,85.8,96.8,4.7,Dropped,NA
STU023,2026-05,Python Programming,Batch-6,Trainer D,Walk-in,Returning,15000,15000,97.3,72.0,64.0,3.7,Completed,Not Placed
STU024,2026-06,Python Programming,Batch-4,Trainer C,Referral,New,20000,20000,86.3,93.3,84.5,3.8,Ongoing,NA
STU025,2026-01,Data Analytics,Batch-2,Trainer C,WhatsApp,New,20000,20000,97.5,95.8,75.7,5.0,Ongoing,NA
STU026,2026-02,Python Programming,Batch-6,Trainer A,Referral,Returning,50000,50000,97.2,61.0,89.8,3.6,Ongoing,NA
STU027,2026-03,Data Analytics,Batch-1,Trainer D,Walk-in,Returning,15000,15000,77.2,57.9,70.3,3.4,Ongoing,NA
STU028,2026-04,Advanced Excel,Batch-6,Trainer B,Instagram,Returning,20000,16078,95.6,70.1,75.0,4.7,Ongoing,NA
STU029,2026-05,Digital Marketing,Batch-2,Trainer A,WhatsApp,New,15000,15000,71.0,55.9,70.4,3.4,Dropped,NA
STU030,2026-06,Python Programming,Batch-1,Trainer A,Referral,New,25000,25000,87.8,75.8,61.2,4.9,Completed,Not Placed
STU031,2026-01,Digital Marketing,Batch-5,Trainer D,Instagram,New,20000,20000,86.1,94.8,81.6,4.4,Completed,Placed
STU032,2026-02,Python Programming,Batch-2,Trainer C,Google,Returning,25000,25000,72.5,90.4,85.0,4.1,Dropped,NA
STU033,2026-03,Digital Marketing,Batch-3,Trainer B,Walk-in,New,15000,15000,81.5,76.0,86.4,3.4,Completed,Placed
STU034,2026-04,AI & Machine Learning,Batch-6,Trainer A,Google,Returning,25000,25000,77.6,91.0,82.6,3.5,Ongoing,NA
STU035,2026-05,Advanced Excel,Batch-6,Trainer D,WhatsApp,New,40000,40000,91.9,64.8,62.4,3.9,Completed,Not Placed
STU036,2026-06,Advanced Excel,Batch-2,Trainer A,Walk-in,New,30000,30000,81.4,91.7,61.4,4.2,Completed,Placed
STU037,2026-01,AI & Machine Learning,Batch-2,Trainer C,Referral,New,20000,11157,73.7,73.2,99.5,4.0,Ongoing,NA
STU038,2026-02,AI & Machine Learning,Batch-5,Trainer D,Google,Returning,15000,15000,81.5,69.0,71.0,4.0,Ongoing,NA
STU039,2026-03,Web Development,Batch-5,Trainer C,Walk-in,Returning,20000,20000,87.1,87.6,97.6,4.9,Completed,Placed
STU040,2026-04,Digital Marketing,Batch-1,Trainer D,Referral,New,30000,30000,86.6,75.3,66.9,3.9,Completed,Placed
STU041,2026-05,Digital Marketing,Batch-6,Trainer A,Instagram,New,15000,15000,96.7,93.6,60.8,4.7,Completed,Placed
STU042,2026-06,Digital Marketing,Batch-2,Trainer D,Walk-in,Returning,25000,17259,92.4,68.8,89.2,4.3,Completed,Not Placed
STU043,2026-01,Advanced Excel,Batch-1,Trainer B,Instagram,New,15000,15000,74.6,68.4,80.3,3.4,Ongoing,NA
STU044,2026-02,Advanced Excel,Batch-4,Trainer A,Google,New,15000,15000,83.2,94.5,88.2,3.7,Ongoing,NA
STU045,2026-03,Web Development,Batch-6,Trainer A,Referral,New,25000,25000,82.9,96.3,79.0,4.2,Completed,Not Placed
STU046,2026-04,AI & Machine Learning,Batch-4,Trainer A,Google,Returning,30000,30000,94.8,88.5,68.6,3.6,Completed,Placed
STU047,2026-05,Web Development,Batch-6,Trainer C,Walk-in,Returning,20000,20000,87.4,55.4,70.1,4.6,Ongoing,NA
STU048,2026-06,Advanced Excel,Batch-1,Trainer A,WhatsApp,Returning,25000,25000,76.3,68.0,80.8,4.3,Ongoing,NA
STU049,2026-01,AI & Machine Learning,Batch-3,Trainer C,Referral,Returning,40000,40000,87.7,67.8,64.3,3.3,Ongoing,NA
STU050,2026-02,AI & Machine Learning,Batch-2,Trainer A,Walk-in,Returning,20000,20000,92.2,93.7,92.2,4.6,Completed,Placed
STU051,2026-03,Python Programming,Batch-3,Trainer B,WhatsApp,Returning,25000,16628,81.3,56.5,88.3,4.2,Ongoing,NA
STU052,2026-04,Web Development,Batch-1,Trainer D,Instagram,Returning,50000,50000,78.7,62.3,86.3,4.2,Ongoing,NA
STU053,2026-05,Web Development,Batch-4,Trainer C,Referral,Returning,50000,44999,96.5,95.7,96.0,4.4,Completed,Placed
STU054,2026-06,Data Analytics,Batch-4,Trainer B,WhatsApp,New,40000,40000,94.7,75.2,94.7,4.3,Ongoing,NA
STU055,2026-01,Python Programming,Batch-3,Trainer D,WhatsApp,Returning,50000,50000,78.7,57.3,94.2,3.4,Ongoing,NA
STU056,2026-02,Data Analytics,Batch-4,Trainer C,Instagram,New,20000,20000,90.8,88.5,79.5,4.3,Completed,Placed
STU057,2026-03,Digital Marketing,Batch-4,Trainer A,Google,New,40000,40000,84.2,87.8,63.5,4.3,Completed,Placed
STU058,2026-04,AI & Machine Learning,Batch-6,Trainer B,Instagram,Returning,50000,50000,70.4,68.9,93.3,3.5,Ongoing,NA
STU059,2026-05,AI & Machine Learning,Batch-5,Trainer C,Walk-in,New,25000,25000,81.1,80.3,66.7,4.7,Completed,Placed
STU060,2026-06,Python Programming,Batch-2,Trainer B,Instagram,New,25000,18031,80.4,63.1,97.9,4.9,Completed,Not Placed
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| Attendance | 80% or higher |
| Test Score | 70 or higher |
| Assignment Completion | 85% or higher |
| Student Satisfaction | 4.2 or higher |
| Course Completion | 85% or higher |
| Placement Rate | 60% or higher |
| Fee Collection | 95% or higher |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **Fee Collection Rate**: `Paid Amount / Course Fee × 100`
- **Course Completion Rate**: `Completed / Total Students × 100`
- **Placement Rate**: `Placed / Completed Students × 100`
- **Average Attendance**: `Average Attendance %`
- **Average Test Score**: `Average Test Score`
- **Average Satisfaction**: `Average Satisfaction`

---

## 6. Assignment Tasks

### Task 1 — Course Performance
Compare courses by enrollment, fee collection, attendance, test score, satisfaction, completion and placement.
### Task 2 — Trainer Performance
Compare trainers by student count, attendance, score, assignment completion and satisfaction.
### Task 3 — Lead Source Analysis
Identify which lead sources generate the most students and highest fee collection.
### Task 4 — Batch Analysis
Compare batches by enrollment, attendance, completion and satisfaction.
### Task 5 — Academic Performance
Analyze the relationship between attendance, assignment completion and test score.
### Task 6 — Fee Collection
Compare Course Fee vs Paid Amount and identify fee collection gaps.
### Task 7 — Placement Analysis
Calculate placement rate by course and trainer for completed students.
### Task 8 — Benchmark Analysis
Classify courses and trainers against attendance, score, satisfaction, completion and placement benchmarks.
### Task 9 — Institute Dashboard
Build a management dashboard with course, trainer and lead-source slicers.
### Task 10 — Management Recommendations
Recommend courses, trainers, lead sources and student-success actions.

---

## 7. Recommended Pivot Charts

1. **Enrollment by Course** — Column Chart
2. **Fee Collection by Course** — Bar Chart
3. **Placement Rate by Course** — Column Chart
4. **Student Source Mix** — Bar/Pie Chart
5. **Monthly Enrollment Trend** — Line Chart
6. **Trainer Performance** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Total Students
- Fee Collection Rate
- Average Attendance
- Average Test Score
- Completion Rate
- Placement Rate
- Average Satisfaction
- Outstanding Fees

### Filters / Slicers

- Course
- Trainer
- Lead_Source
- Batch
- Student_Type

### Dashboard Charts

- Enrollment by Course
- Placement Rate by Course
- Fee Collection by Course
- Monthly Enrollment Trend

---

## 9. Final Business Questions

1. Which course has the highest enrollment?
2. Which course collects the most fees?
3. Which trainer has the strongest student outcomes?
4. Which lead source generates the most students?
5. Which course has the highest placement rate?
6. Which course falls below the attendance benchmark?
7. Where are fee collection gaps highest?
8. Which KPI should the institute prioritize?
9. What three actions could improve completion and placement?

---

## 10. Final Management Challenge

Management wants to improve student outcomes and revenue simultaneously. Identify which courses and trainers are strongest, where students are dropping off, and which acquisition channels deserve more attention.

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
