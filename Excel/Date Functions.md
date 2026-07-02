# Excel Practical Assignment: Date Functions

## Objective

Use Excel Date Functions to create, extract, calculate, and format dates using:

* TODAY
* NOW
* DATE
* DAY
* MONTH
* YEAR
* WEEKDAY
* TEXT
* EDATE
* EOMONTH
* DATEDIF

---

# Dataset

Enter the following data in Excel:

| Employee ID | Employee Name | Joining Date | Birth Date | Project Start | Project End |
| ----------- | ------------- | ------------ | ---------- | ------------- | ----------- |
| 101         | Aditi Sharma  | 12-01-2023   | 15-05-2000 | 05-07-2026    | 20-08-2026  |
| 102         | Rahul Verma   | 18-03-2022   | 20-10-1998 | 10-07-2026    | 15-09-2026  |
| 103         | Neha Gupta    | 25-08-2021   | 12-01-1999 | 18-07-2026    | 30-09-2026  |
| 104         | Arjun Singh   | 30-11-2024   | 08-12-2001 | 25-07-2026    | 05-10-2026  |
| 105         | Kavya Mehta   | 14-06-2020   | 22-03-1997 | 01-08-2026    | 15-10-2026  |

---

# Part A: Basic Date Functions

Perform the following operations:

1. Display the current date using **TODAY()**
2. Display the current date and time using **NOW()**
3. Create a new date using the **DATE()** function (Example: 15-Aug-2026)
4. Extract the **Day** from Joining Date.
5. Extract the **Month** from Joining Date.
6. Extract the **Year** from Joining Date.

---

# Part B: Date Analysis

Create the following columns:

7. Display the weekday number using **WEEKDAY()**.
8. Display the weekday name (Monday, Tuesday, etc.) using **TEXT()**.
9. Display the month name using **TEXT()**.
10. Display the month abbreviation (Jan, Feb, etc.).

---

# Part C: Date Calculations

11. Add 3 months to the Project Start Date using **EDATE()**.
12. Find the last day of the Joining Date month using **EOMONTH()**.
13. Find the last day of the next month using **EOMONTH()**.
14. Calculate the total number of days between Project Start and Project End.
15. Calculate years of service from Joining Date to today's date.

---

# Part D: DATEDIF Function

Using **DATEDIF()**, calculate:

16. Employee Age in Years.
17. Employee Age in Months.
18. Employee Age in Days.
19. Total Years of Service.
20. Remaining Months after completed Years of Service.

---

# Part E: Date Formatting

Use the **TEXT()** function to display dates in the following formats:

21. dd-mmm-yyyy (Example: 12-Jan-2026)
22. dd/mm/yyyy
23. mmmm dd, yyyy
24. dddd (Full weekday name)
25. mmmm (Full month name)

---

# Part F: Practical Challenges

26. Find the number of days left until the Project Start Date.
27. Find the number of days remaining until the Project End Date.
28. Display **"Expired"** if Project End Date is earlier than TODAY(), otherwise display **"Active"**.
29. Display **"Weekend"** if Joining Date falls on Saturday or Sunday; otherwise display **"Weekday"**.
30. Create a summary using CONCAT:

**Employee Name + " joined on " + Joining Date + " and project ends on " + Project End Date**

Example Output:

Aditi Sharma joined on 12-Jan-2023 and project ends on 20-Aug-2026

---

# Bonus Practice

31. Find the first day of the current month.
32. Find the last day of the current month.
33. Display today's date as:

* 02-Jul-2026
* Thursday
* July
* Q3 (Quarter)

34. Calculate the number of weekends between Project Start and Project End.
35. Find the employee with the earliest Joining Date.
