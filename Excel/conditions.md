# Excel Practical Assignment: IF(), AND(), OR(), Nested IF(), IFS(), IFERROR()

## Objective

Practice Excel logical functions by solving real-world business problems using:

- IF()
- AND()
- OR()
- Nested IF()
- IFS()
- IFERROR()

---

# Dataset

Enter the following data into Excel.

| Emp ID | Employee | Department | Sales | Target | Attendance % | Experience (Years) | Salary | Bonus Eligible | Errors |
|--------:|----------------|------------|------:|-------:|-------------:|-------------------:|-------:|----------------|-------:|
| 101 | Aditi Sharma | Sales | 65000 | 60000 | 96 | 5 | 45000 | Yes | 25 |
| 102 | Rahul Verma | HR | 42000 | 45000 | 88 | 2 | 38000 | No | 0 |
| 103 | Neha Gupta | Sales | 78000 | 70000 | 99 | 7 | 55000 | Yes | 12 |
| 104 | Arjun Singh | IT | 39000 | 40000 | 82 | 1 | 35000 | No | 8 |
| 105 | Kavya Mehta | Sales | 85000 | 80000 | 97 | 9 | 62000 | Yes | 3 |
| 106 | Rohan Patel | Finance | 58000 | 60000 | 90 | 4 | 47000 | Yes | 15 |
| 107 | Simran Kaur | IT | 72000 | 70000 | 95 | 6 | 54000 | Yes | 0 |
| 108 | Aman Gupta | HR | 36000 | 40000 | 78 | 1 | 33000 | No | 20 |
| 109 | Priya Shah | Sales | 91000 | 85000 | 98 | 10 | 70000 | Yes | 2 |
| 110 | Mohit Jain | Finance | 51000 | 50000 | 91 | 3 | 43000 | Yes | 5 |

---

# Part A – IF() Function (10 Questions)

Use only the **IF()** function.

### Question 1
Display **Achieved** if Sales is greater than or equal to Target; otherwise display **Not Achieved**.

### Question 2
If Attendance is 90% or above, display **Present**; otherwise display **Needs Improvement**.

### Question 3
If Salary is greater than ₹50,000, display **High Salary**; otherwise display **Normal Salary**.

### Question 4
If Errors are equal to 0, display **Perfect Work**; otherwise display **Check Errors**.

### Question 5
If Experience is 5 years or more, display **Experienced**; otherwise display **Beginner**.

### Question 6
If Bonus Eligible is **Yes**, display **Bonus Approved**; otherwise display **No Bonus**.

### Question 7
If Sales are greater than ₹80,000, return a Bonus of **₹5,000**; otherwise return **₹0**.

### Question 8
If Department is **Sales**, display **Sales Team**; otherwise display **Other Department**.

### Question 9
If Attendance is less than 80%, display **Warning**; otherwise display **OK**.

### Question 10
If Salary is less than ₹40,000, display **Increment Required**; otherwise display **No Action**.

---

# Part B – AND() Function (10 Questions)

Use **AND()** together with **IF()**.

### Question 1
Display **Eligible for Promotion** only if:
- Attendance is at least 95%
- Experience is at least 5 years

### Question 2
Display **Bonus Approved** only if:
- Sales are greater than or equal to Target
- Bonus Eligible is Yes

### Question 3
Display **Excellent Employee** only if:
- Sales are at least ₹70,000
- Attendance is at least 95%

### Question 4
Display **Top Performer** only if:
- Salary is greater than ₹50,000
- Experience is greater than 5 years

### Question 5
Display **Safe Employee** only if:
- Errors are fewer than 5
- Attendance is at least 90%

### Question 6
Display **Senior Salesperson** only if:
- Department is Sales
- Experience is at least 7 years

### Question 7
Display **Reward** only if:
- Sales are greater than ₹80,000
- Attendance is greater than 95%

### Question 8
Display **Reliable** only if:
- Errors are 0
- Attendance is 100%

### Question 9
Display **Leadership Candidate** only if:
- Experience is greater than 8 years
- Sales are greater than ₹85,000

### Question 10
Display **Excellent Discipline** only if:
- Attendance is greater than 95%
- Errors are fewer than 5

---

# Part C – OR() Function (10 Questions)

Use **OR()** together with **IF()**.

### Question 1
Display **Eligible** if:
- Sales are greater than or equal to Target
- OR Attendance is at least 95%

### Question 2
Display **Bonus Approved** if:
- Department is Sales
- OR Department is Finance

### Question 3
Display **Training Required** if:
- Attendance is below 85%
- OR Errors are greater than 15

### Question 4
Display **Senior Employee** if:
- Experience is at least 8 years
- OR Salary is greater than ₹60,000

### Question 5
Display **Needs Review** if:
- Sales are below ₹40,000
- OR Errors are greater than 10

### Question 6
Display **Priority Employee** if:
- Department is IT
- OR Department is Sales

### Question 7
Display **High Performer** if:
- Sales are greater than ₹80,000
- OR Attendance is greater than 98%

### Question 8
Display **Good Employee** if:
- Salary is greater than ₹50,000
- OR Experience is greater than 6 years

### Question 9
Display **Special Recognition** if:
- Errors are 0
- OR Sales are greater than ₹90,000

### Question 10
Display **Management Review** if:
- Attendance is below 80%
- OR Salary is below ₹35,000

---

# Part D – Nested IF() Function (10 Questions)

### Question 1 – Performance Rating

- Sales ≥ 80,000 → Excellent
- Sales ≥ 60,000 → Good
- Otherwise → Average

### Question 2 – Attendance Grade

- ≥95 → A
- ≥90 → B
- ≥80 → C
- Otherwise → D

### Question 3 – Experience Level

- ≥8 → Expert
- ≥5 → Senior
- ≥2 → Intermediate
- Otherwise → Fresher

### Question 4 – Salary Grade

- >60,000 → Grade A
- >50,000 → Grade B
- >40,000 → Grade C
- Otherwise → Grade D

### Question 5 – Error Level

- 0 → Perfect
- ≤5 → Minor
- ≤15 → Moderate
- Otherwise → Critical

### Question 6 – Sales Commission

- ≥90,000 → 15%
- ≥70,000 → 10%
- ≥50,000 → 5%
- Otherwise → 0%

### Question 7 – Attendance Status

- 100 → Outstanding
- ≥95 → Excellent
- ≥90 → Good
- Otherwise → Needs Improvement

### Question 8 – Promotion Level

- Experience ≥10 → Immediate
- Experience ≥7 → High Priority
- Experience ≥5 → Consider
- Otherwise → Not Eligible

### Question 9 – Department Category

- Sales → Revenue
- HR → Support
- IT → Technical
- Otherwise → Administration

### Question 10 – Risk Level

- Errors >20 → High
- Errors >10 → Medium
- Errors >5 → Low
- Otherwise → Safe

---

# Part E – IFS() Function (10 Questions)

Use **IFS()** instead of Nested IF() wherever applicable.

### Question 1
Assign Performance Rating.

### Question 2
Assign Attendance Grade.

### Question 3
Assign Salary Grade.

### Question 4
Assign Experience Level.

### Question 5
Assign Error Severity.

### Question 6
Assign Commission Percentage.

### Question 7
Assign Promotion Priority.

### Question 8
Assign Employee Category based on Salary.

### Question 9
Assign Sales Category.

- Above ₹90,000
- Above ₹70,000
- Above ₹50,000
- Below ₹50,000

### Question 10
Assign Attendance Status.

- Excellent
- Good
- Average
- Poor

---

# Part F – IFERROR() Function (10 Questions)

### Question 1
Calculate **Sales ÷ Target** and display **"Invalid Calculation"** if an error occurs.

### Question 2
Calculate **Salary ÷ Errors**. If Errors are zero, display **"No Errors"**.

### Question 3
Calculate **Target ÷ Sales**. If an error occurs, display **"Invalid"**.

### Question 4
Calculate **Sales ÷ Attendance**. If an error occurs, return **0**.

### Question 5
Calculate **Bonus Amount ÷ Errors**. If an error occurs, display **"Not Applicable"**.

### Question 6
Use **VLOOKUP()** or **XLOOKUP()** to find an Employee by ID. If not found, display **"Employee Not Found"**.

### Question 7
Find Salary using a lookup function. If not found, display **"No Record"**.

### Question 8
Calculate **Experience ÷ Errors**. If an error occurs, display **"Cannot Calculate"**.

### Question 9
Lookup Department using Employee ID. If lookup fails, display **"Department Missing"**.

### Question 10
Calculate **(Sales + Salary) ÷ Errors**. If an error occurs, display **"No Division Possible"**.

---

# Bonus Challenge

Create an **Employee Performance Dashboard** using Excel formulas and charts that displays:

- Total Employees
- Employees Who Achieved Target
- Employees Who Did Not Achieve Target
- Average Sales
- Highest Sales
- Lowest Sales
- Employees Eligible for Promotion
- Employees Receiving Bonus
- Average Attendance
- Total Salary Paid
- Employee with Highest Sales
- Error-Free Employees

---
**End of Assignment**
