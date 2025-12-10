# Summary of Data Cleaning – Superstore Task 2

## ✔ 1. Removed Duplicate Records
Checked for repeated rows using:
- order_id  
- product_id  
- customer_id  

No exact duplicates remained after cleaning.

---

## ✔ 2. Fixed Data Types
Converted column types properly:

| Column         | Correct Type |
|----------------|--------------|
| order_date     | Date         |
| ship_date      | Date         |
| discount       | Decimal      |
| sales          | Decimal      |
| profit         | Decimal      |
| quantity       | Whole Number |
| shipping_cost  | Decimal      |

This ensured accurate calculations and visuals in Power BI.

---

## ✔ 3. Text Standardization
- Trimmed extra spaces from text columns  
- Standardized casing (e.g., “Furniture”, “Office Supplies”)  
- Cleaned inconsistent naming in **state**, **city**, **sub_category**

---

## ✔ 4. Missing Value Handling
- Verified missing values in **sales**, **profit** → none found  
- Missing discount values (if any) were filled with **0**  
- No missing dates after cleaning  

---

## ✔ 5. Removed Unnecessary Columns
Removed fields not needed for analysis:
- row_id  
- weeknum  
- market2  

These did not contribute to dashboard insights.

---

## ✔ 6. Added Derived Columns (If Required for Dashboard)
Created:
- Profit Margin %  
- Loss Amount (profit < 0)  

Defined using DAX inside Power BI.

---

## ✔ 7. Verified Consistency
- Ensured order_date < ship_date  
- Verified region/category alignment  
- Confirmed negative profits represent actual losses  

---

### 📝 Final Note
This cleaned dataset was used to build the Power BI dashboard for Task 2, supporting the narrative:  
**“Profit is hiding in plain sight — identifying products & regions killing growth.”**
