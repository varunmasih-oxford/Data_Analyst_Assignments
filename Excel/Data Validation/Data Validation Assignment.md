# Sales Dataset -- Data Validation Concepts

## Dataset Overview

This dataset contains 100 sales transaction records with real-life
business fields.

### Columns Included

1.  Sale_ID -- Unique transaction ID (S0001--S0100)\
2.  Sale_Date -- Date of sale (2024 range)\
3.  Customer_ID -- Customer reference (C001--C050)\
4.  Product_Name -- Product sold\
5.  Category -- Product category\
6.  Region -- Sales region\
7.  Quantity -- Units sold\
8.  Unit_Price -- Price per unit\
9.  Discount_Percent -- Discount applied (%)\
10. Discount_Amount -- Calculated discount value\
11. Total_Amount -- Final payable amount\
12. Payment_Method -- Mode of payment

------------------------------------------------------------------------

# Real-Life Data Validation Concepts

## 1. Required Field Validation

-   Sale_ID → Cannot be blank\
-   Sale_Date → Cannot be empty\
-   Customer_ID → Required\
-   Quantity → Required\
-   Unit_Price → Required

------------------------------------------------------------------------

## 2. Data Type Validation

  Column             Expected Type
  ------------------ ---------------
  Sale_ID            Text
  Sale_Date          Date
  Customer_ID        Text
  Quantity           Whole Number
  Unit_Price         Decimal
  Discount_Percent   Number
  Discount_Amount    Decimal
  Total_Amount       Decimal

------------------------------------------------------------------------

## 3. Range Validation

### Quantity

-   Minimum: 1\
-   Maximum: 100

### Discount Percent

-   Minimum: 0\
-   Maximum: 50

### Unit Price

-   Must be greater than 0

------------------------------------------------------------------------

## 4. Lookup / List Validation (Dropdown)

### Region (Allowed Values Only)

-   North\
-   South\
-   East\
-   West

### Payment Method

-   Cash\
-   Credit Card\
-   UPI\
-   Net Banking

### Category

-   Electronics\
-   Furniture\
-   Accessories

------------------------------------------------------------------------

## 5. Unique Validation

-   Sale_ID must be unique\
-   No duplicate transaction IDs allowed

------------------------------------------------------------------------

## 6. Referential Integrity

-   Customer_ID must exist in Customer Master table\
-   Product_Name must exist in Product Master table

------------------------------------------------------------------------

## 7. Formula Validation

### Discount Formula

Discount_Amount = (Unit_Price × Quantity) × (Discount_Percent / 100)

### Total Amount Formula

Total_Amount = (Unit_Price × Quantity) - Discount_Amount

------------------------------------------------------------------------

## 8. Logical Validation

-   Discount_Amount cannot exceed total sales value\
-   Total_Amount must be ≥ 0\
-   Sale_Date cannot be future date\
-   If Discount_Percent = 0 → Discount_Amount must be 0

------------------------------------------------------------------------

## 9. Format Validation

### Sale_ID Pattern

\^S`\d{4}`{=tex}\$

### Customer_ID Pattern

\^C`\d{3}`{=tex}\$

------------------------------------------------------------------------

## 10. Cross Field Validation

-   If Category = Electronics → Unit_Price \> 1000\
-   If Payment_Method = Credit Card → Transaction ID required (if added)

------------------------------------------------------------------------

## 11. Business Rule Validation

-   Discount \> 30% requires approval\
-   Quantity \> 8 flagged as wholesale\
-   Total_Amount \> 200000 flagged as high-value sale

------------------------------------------------------------------------

## 12. Duplicate Detection

Check duplicates on: - Sale_ID\
- Combination of (Customer_ID + Sale_Date + Product_Name)


