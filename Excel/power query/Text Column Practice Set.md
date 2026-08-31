# Assignment: Power Query — Text Column Practice Set

## Dataset: Sales_Data

Use the same `Sales_Data` dataset from the previous assignment.

### Objective

Practice the following Power Query Text Column options:

- Split Column
- Format
- Merge Columns
- Extract

> **Important:** Complete the exercises using Power Query transformations. Do not manually edit the source data.

---

# Level 1 — Split Column

## Task 1: Split City and Region

Create a new column called:

`City_Region`

Combine `City` and `Region` first using a hyphen.

Example:

| City | Region | City_Region |
|---|---|---|
| Delhi | North | Delhi-North |
| Mumbai | West | Mumbai-West |

Then use **Split Column → By Delimiter** to split `City_Region` back into:

- City
- Region

**Delimiter:** `-`

---

## Task 2: Split Product Information

Create a new column by combining:

`Category` + `Product`

Use a hyphen as the separator.

Example:

`Electronics-Laptop`

Then split the column into:

| Category | Product |
|---|---|
| Electronics | Laptop |

---

## Task 3: Split Salesperson Name

Create a new column:

`Salesperson_Code`

Combine the salesperson name with a code.

Example:

`Amit-001`

Then use **Split Column → By Delimiter** to separate:

| Salesperson | Code |
|---|---|
| Amit | 001 |

---

## Task 4: Split Product Name by Character Position

Use the `Product` column.

Split the product name using **Split Column → By Number of Characters**.

Try:

- Split into the first 2 characters
- Split the remaining characters

Example:

`Laptop`

Result:

| Part 1 | Part 2 |
|---|---|
| La | ptop |

---

## Task 5: Split Date Text

Convert the `Date` column to Text.

Then use **Split Column → By Delimiter** using `-`.

Create:

| Day | Month | Year |
|---|---|---|
| 01 | 01 | 2026 |

Use the three resulting columns to understand how text-based date splitting works.

---

# Level 2 — Format

## Task 6: Convert Salesperson Names to Uppercase

Use:

**Transform → Format → UPPERCASE**

Expected result:

| Original | Formatted |
|---|---|
| Amit | AMIT |
| Neha | NEHA |
| Rahul | RAHUL |
| Priya | PRIYA |
| Suresh | SURESH |

---

## Task 7: Convert Product Names to Lowercase

Use:

**Transform → Format → lowercase**

Expected result:

| Original | Formatted |
|---|---|
| Laptop | laptop |
| Mobile | mobile |
| Chair | chair |
| Table | table |
| Rice | rice |
| Oil | oil |

---

## Task 8: Apply Capitalization

Use:

**Transform → Format → Capitalize Each Word**

Apply it to the `Salesperson` column.

Expected:

`AMIT` → `Amit`

`NEHA` → `Neha`

`RAHUL` → `Rahul`

---

## Task 9: Clean Text

Create a copy of the `Product` column.

Use:

**Transform → Format → Clean**

The objective is to remove non-printing characters from text.

---

## Task 10: Trim Text

Create a copy of the `City` column.

Use:

**Transform → Format → Trim**

The objective is to remove unnecessary spaces from the beginning and end of text values.

---

## Task 11: Clean and Trim

Create a new text column containing:

`Salesperson + " " + Product`

Then apply:

1. Clean
2. Trim

This exercise demonstrates how multiple text-cleaning transformations can be applied sequentially.

---

# Level 3 — Merge Columns

## Task 12: Merge Salesperson and Region

Merge:

- Salesperson
- Region

Use `_` as the separator.

Expected:

| Salesperson | Region | Result |
|---|---|---|
| Amit | North | Amit_North |
| Rahul | West | Rahul_West |
| Priya | South | Priya_South |

---

## Task 13: Merge City and Region

Merge:

- City
- Region

Use `-` as the separator.

Expected:

`Delhi-North`

`Mumbai-West`

`Bangalore-South`

---

## Task 14: Merge Category and Product

Merge:

- Category
- Product

Use ` / ` as the separator.

Expected:

| Category | Product | Result |
|---|---|---|
| Electronics | Laptop | Electronics / Laptop |
| Furniture | Chair | Furniture / Chair |
| Grocery | Rice | Grocery / Rice |

---

## Task 15: Create a Product Description

Merge:

- Category
- Product
- Salesperson

Use ` | ` as the separator.

Example:

`Electronics | Laptop | Amit`

Create the following column:

`Product_Description`

---

## Task 16: Create an Order Label

Merge:

- Order_ID
- Product

Use `-` as the separator.

Example:

`1001-Laptop`

Create:

`Order_Label`

---

## Task 17: Create a Location Label

Merge:

- Region
- City

Use `, ` as the separator.

Example:

`North, Delhi`

Create:

`Location`

---

# Level 4 — Extract

## Task 18: Extract First Characters

Use the `Product` column.

Apply:

**Extract → First Characters**

Extract the first **3 characters**.

Expected examples:

| Product | First 3 Characters |
|---|---|
| Laptop | Lap |
| Mobile | Mob |
| Chair | Cha |
| Table | Tab |
| Rice | Ric |
| Oil | Oil |

---

## Task 19: Extract Last Characters

Use the `Product` column.

Extract the last **2 characters**.

Expected examples:

| Product | Last 2 Characters |
|---|---|
| Laptop | op |
| Mobile | le |
| Chair | ir |
| Table | le |
| Rice | ce |
| Oil | il |

---

## Task 20: Extract Text Before Delimiter

Use the `Order_Label` created in Task 16.

Example:

`1001-Laptop`

Use:

**Extract → Text Before Delimiter**

Delimiter:

`-`

Expected result:

`1001`

---

## Task 21: Extract Text After Delimiter

Use the same `Order_Label`.

Example:

`1001-Laptop`

Use:

**Extract → Text After Delimiter**

Delimiter:

`-`

Expected result:

`Laptop`

---

## Task 22: Extract Text Between Delimiters

Create a column:

`Region-Category-Product`

Example:

`North-Electronics-Laptop`

Use:

**Extract → Text Between Delimiters**

Extract the text between:

First delimiter: `-`

Second delimiter: `-`

Expected:

`Electronics`

---

## Task 23: Extract Text Range

Use the `Product` column.

Use:

**Extract → Range**

Experiment with:

- Starting position
- Number of characters

For example:

`Laptop`

Starting position: `1`

Number of characters: `3`

Result:

`Lap`

---

# Level 5 — Combined Text Transformations

## Task 24: Create a Business Key

Create a new column called:

`Business_Key`

Use:

- Region
- Category
- Product

Merge them using `_`.

Example:

`North_Electronics_Laptop`

Then:

1. Convert the result to uppercase.
2. Extract the first 10 characters.
3. Create a final column called `Business_Key_Short`.

---

## Task 25: Create an Order Description

Create a final column called:

`Order_Description`

Combine:

- Order_ID
- Date
- Region
- City
- Salesperson
- Product

Use ` | ` as the separator.

Example:

`1001 | 01-01-2026 | North | Delhi | Amit | Laptop`

Then apply appropriate text formatting.

---

# Level 6 — Business Reporting Practice

## Task 26: Create Salesperson Region Code

Create:

`Salesperson_Region`

Combine:

`Salesperson + Region`

Example:

`Amit-North`

Then extract:

- Salesperson
- Region

into separate columns.

---

## Task 27: Create Product Category Code

Create:

`Product_Code`

Combine:

`Category + Product`

Example:

`Electronics-Laptop`

Convert it to uppercase.

Expected:

`ELECTRONICS-LAPTOP`

---

## Task 28: Create City Code

Use the `City` column.

Extract the first **3 characters**.

Create:

`City_Code`

Examples:

| City | City Code |
|---|---|
| Delhi | DEL |
| Mumbai | MUM |
| Bangalore | BAN |
| Chennai | CHE |
| Kolkata | KOL |
| Patna | PAT |
| Noida | NOI |
| Pune | PUN |

Convert the result to uppercase.

---

## Task 29: Create Product Code

Use the first 3 characters of `Product` and first 2 characters of `Category`.

Create a combined code.

Example:

`Laptop + Electronics`

Result:

`LAPEL`

Create:

`Product_Code`

---

## Task 30: Create a Complete Order Reference

Create:

`Order_Reference`

Combine:

- Region
- City
- Salesperson
- Product
- Order_ID

Use `-` as the separator.

Example:

`North-Delhi-Amit-Laptop-1001`

Then apply:

1. Uppercase
2. Extract the first 15 characters
3. Create `Short_Order_Reference`

---

# Challenge Tasks

## Challenge 1: Create a Unique Product Key

Create:

`Region_Product_Key`

Example:

`NORTH_LAPTOP`

Requirements:

1. Merge Region and Product.
2. Use `_` as separator.
3. Convert to uppercase.
4. Remove unnecessary spaces.

---

## Challenge 2: Create a Salesperson Code

Create a code using:

- First 3 characters of Salesperson
- First 2 characters of Region

Example:

`Amit + North`

Result:

`AMINO`

Create:

`Salesperson_Code`

---

## Challenge 3: Create a Location Code

Create a code using:

- First 3 characters of City
- First 2 characters of Region

Example:

`Delhi + North`

Result:

`DELNO`

Convert the final code to uppercase.

---

## Challenge 4: Product Identification

Create a column:

`Product_ID`

Use:

- First 3 characters of Category
- First 3 characters of Product

Example:

`Electronics + Laptop`

Result:

`ELELAP`

Convert the final result to uppercase.

---

## Challenge 5: Complete Customer-Style Label

Although the dataset does not contain a Customer column, create a business-style label using:

- Salesperson
- City
- Region
- Product

Example:

`Amit | Delhi | North | Laptop`

Then:

1. Merge the columns.
2. Apply proper capitalization.
3. Remove unnecessary spaces.
4. Extract the Product portion into a separate column.
5. Create a final clean label.

---

# Submission Requirements

For each task:

1. Load `Sales_Data` into Power Query.
2. Create a duplicate query or reference query for practice.
3. Use the appropriate Text Column transformation.
4. Rename columns clearly.
5. Keep the original source columns unchanged wherever possible.
6. Apply transformations in the correct order.
7. Load the final result back to Excel.
8. Keep each exercise as a separate query where appropriate.
9. Do not manually modify the source dataset.

---

# Power Query Skills Covered

## Split Column

- By Delimiter
- By Number of Characters
- By Positions

## Format

- UPPERCASE
- lowercase
- Capitalize Each Word
- Trim
- Clean

## Merge Columns

- Merge two columns
- Merge multiple columns
- Custom separators
- Create business keys
- Create labels

## Extract

- First Characters
- Last Characters
- Text Before Delimiter
- Text After Delimiter
- Text Between Delimiters
- Range

## Combined Skills

- Text transformation
- Column merging
- Column splitting
- Text extraction
- Text cleaning
- Text formatting
- Business key creation
- Code creation
- Data preparation
