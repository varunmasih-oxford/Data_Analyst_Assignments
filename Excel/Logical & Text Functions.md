# Excel Practical Assignment: Logical & Text Functions

## Objective

Use Excel functions to clean, analyze, and format data using:

* IF function
* TEXT functions (UPPER, LOWER, TRIM, LEN, LEFT, RIGHT, MID, REPLACE, SUBSTITUTE, CONCAT)
* Conditional Formatting

---

## Dataset

Enter the following data in Excel:

| ID | Full Name    | Email                                       | Phone Number | Region Code | Sales | Target | Date       |
| -- | ------------ | ------------------------------------------- | ------------ | ----------- | ----- | ------ | ---------- |
| 1  | aditi sharma | [ADITI@GMAIL.COM](mailto:ADITI@GMAIL.COM)   | 98765 43210  | IND-DEL-001 | 52000 | 50000  | 12-01-2026 |
| 2  | rahul verma  | [rahul@Yahoo.com](mailto:rahul@Yahoo.com)   | 91234 56789  | IND-MUM-002 | 43000 | 45000  | 15-01-2026 |
| 3  | NEHA GUPTA   | [NEHA@OUTLOOK.COM](mailto:NEHA@OUTLOOK.COM) | 99887 66554  | IND-KOL-003 | 61000 | 60000  | 18-01-2026 |
| 4  | arjun  singh | [ARJUN@GMAIL.COM](mailto:ARJUN@GMAIL.COM)   | 98700 11223  | IND-DEL-004 | 39000 | 40000  | 20-01-2026 |
| 5  | kavya mehta  | [Kavya@Gmail.Com](mailto:Kavya@Gmail.Com)   | 90909 80808  | IND-AHM-005 | 75000 | 70000  | 22-01-2026 |

---

## Part A: Text Functions

Perform the following operations:

1. Remove extra spaces from "Full Name"
2. Convert names into uppercase
3. Convert emails into lowercase
4. Count total characters in each name
5. Extract the first name
6. Extract last 4 digits of phone number
7. Extract city/state code from Region Code
8. Replace "IND" with "USA"
9. Replace "gmail.com" (any case) with "company.com"
10. Combine Name and Phone Number

---

## Part B: IF Functions (Apply Conditions)

Create the following columns based on given conditions:

11. Status

* Compare Sales and Target
* If Sales is greater than or equal to Target → Achieved
* Otherwise → Not Achieved

12. Bonus

* If Sales is greater than or equal to Target → 10% of Sales
* Otherwise → 0

13. Performance Level

* If Sales is greater than or equal to 70000 → Excellent
* If Sales is greater than or equal to 50000 → Good
* Otherwise → Average

---

## Part C: TEXT Function Formatting

14. Format Date as dd-mmm-yyyy
15. Display Sales with ₹ symbol using TEXT function

---

## Part D: Conditional Formatting

Apply the following rules:

16. Highlight "Achieved" in green
17. Highlight "Not Achieved" in red
18. Highlight Sales less than 40000
19. Highlight top 2 Sales values
20. Highlight duplicate Region Codes

---

## Part E: Advanced Challenges

21. Mask phone number (show only last 4 digits)
22. Clean email (lowercase and trimmed)
23. Extract only state code (DEL, MUM, etc.)
24. Create summary text (example: Name + Region + Status)

