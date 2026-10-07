# Text DAX Functions Applied on Dataset

Dataset Columns:
- OrderID
- OrderDate
- CustomerName
- Category
- Product
- Quantity
- UnitPrice
- Cost
- City

---

## 1. Concatenation Functions

### CONCATENATE()
```DAX
Customer City = CONCATENATE(Orders[CustomerName], " - " & Orders[City])
```

### CONCATENATEX()
```DAX
All Products = CONCATENATEX(Orders, Orders[Product], ", ")
```

---
## 2. Case Functions

### UPPER()
```DAX
Customer Upper = UPPER(Orders[CustomerName])
```

### LOWER()
```DAX
Category Lower = LOWER(Orders[Category])
```

### PROPER()
```DAX
Proper Product = PROPER(Orders[Product]) -- ?
```

---
## 3. Length & Extraction

### LEN()
```DAX
Customer Length = LEN(Orders[CustomerName])
```

### LEFT()
```DAX
Order Prefix = LEFT(Orders[OrderID], 2)
```

### RIGHT()
```DAX
Category Ending = RIGHT(Orders[Category], 3)
```

### MID()
```DAX
Product Middle = MID(Orders[Product], 2, 3)
```

---
## 4. Search Functions

### SEARCH()
```DAX
Find A in Customer = SEARCH("a", Orders[CustomerName],, 0)
```

### FIND()
```DAX
Find P in Product = FIND("P", Orders[Product],, 0)
```

---
## 5. Clean & Trim

### TRIM()
```DAX
Clean Customer = TRIM(Orders[CustomerName])
```

### CLEAN()
```DAX
City Clean = CLEAN(Orders[City])
```

---
## 6. Replace & Substitute

### SUBSTITUTE()
```DAX
Replace Space = SUBSTITUTE(Orders[CustomerName], " ", "_")
```

### REPLACE()
```DAX
Mask Customer = REPLACE(Orders[CustomerName], 1, 3, "***")
```

---
## 7. Format & Value

### FORMAT()
```DAX
Formatted Date = FORMAT(Orders[OrderDate], "DD-MMM-YYYY")
```

### VALUE()
```DAX
OrderID Number = VALUE(Orders[OrderID])
```

---
## 8. Exact

### EXACT()
```DAX
Is Electronics = EXACT(Orders[Category], "Electronics")
```

---
## 9. Unicode

### UNICODE()
```DAX
Unicode First Letter = UNICODE(LEFT(Orders[CustomerName], 1))
```

### UNICHAR()
```DAX
Star Symbol = UNICHAR(9733)
```

---
## 10. Real-World Text DAX

### City & Category Tag
```DAX
City Category Tag = Orders[City] & " | " & Orders[Category]
```

### Product Short Code
```DAX
Product Code =
UPPER(LEFT(Orders[Product], 3)) & "-" & FORMAT(Orders[OrderID], "0000")
```

### Customer Initials
```DAX
Customer Initials =
LEFT(Orders[CustomerName],1) & MID(Orders[CustomerName], SEARCH(" ", Orders[CustomerName])+1, 1)
```

### Order Description
```DAX
Order Description =
Orders[CustomerName] & " bought " & Orders[Product] & " (" & Orders[Category] & ")"
```

