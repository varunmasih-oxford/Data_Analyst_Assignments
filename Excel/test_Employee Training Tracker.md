# Employee Training Tracker - Assignment

## Scenario
You are an HR analyst at **TechNova Solutions**. The company wants to track employee training programs, completion dates, and training scores. Your task is to clean the dataset, calculate key metrics, and generate insights using Excel.

---

## Dataset Structure

| Employee ID | Full Name        | Department    | Training Program     | Training Start Date | Training End Date | Completion Status | Training Score | Training Cost |
|------------|----------------|--------------|-------------------|------------------|----------------|-----------------|---------------|---------------|
| E101       | John Doe       | IT           | Excel Advanced      | 01-02-2026       | 05-02-2026     | Completed       | 85            | 500           |
| E102       | Jane Smith     | Marketing    | Digital Marketing   | 03-02-2026       | 07-02-2026     | Completed       | 90            | 450           |
| E103       | Alex Johnson   | HR           | Workplace Safety    | 02-02-2026       | 04-02-2026     | Pending         |               | 300           |
| E104       | Emily Davis    | IT           | Power BI            | 04-02-2026       | 10-02-2026     | Completed       | 92            | 600           |
| E105       | Michael Brown  | Finance      | Excel Basics        | 01-02-2026       | 03-02-2026     | Completed       | 78            | 400           |

> **Note:** Extend this dataset to 20–30 rows for practice.

---

## Tasks

### Part 1: Work with Text
1. Extract the **first name** from the full name into a new column.  
2. Extract the **last name** from the full name into a new column.  
3. Create an **email ID** in the format: `firstnamelastname@technova.com`.  

---

### Part 2: Work with Dates
1. Calculate **how many days each training lasted**.  
2. Highlight employees whose **training will finish within the next 3 days**.  
3. Extract the **month** and **year** when the training ended.  

---

### Part 3: Look Up Information
1. Find the **department** for a specific employee ID (`E104`).  
2. Find the **training score** of a specific employee ("Jane Smith").  
3. Find the **training program** for a specific employee ID (`E103`).  

---

### Part 4: Analyze the Data
1. Count how many employees have **completed their training**.  
2. Find the **average training score** for a specific department (e.g., IT).  
3. Find the **total training cost** for a specific department (e.g., Marketing).  
4. Count how many employees scored **above 85**.  
5. Calculate the **average score of employees who completed training**.  
6. Create a **performance status** column:  
   - If training is completed and score ≥ 85 → "Excellent"  
   - If training is completed and score < 85 → "Good"  
   - If training is pending → "Pending"  

---

### Optional Visualization
1. Create a **bar chart** showing average training score by department.  
2. Create a **pie chart** showing the number of completed vs pending trainings.  

---

## Deliverables
1. Excel file with formulas applied (not just values).  
2. Screenshots of charts and key results.  
3. Short summary report (1–2 paragraphs) with insights (e.g., which department spends most on training, trends in scores).  
