# 🧹 Retail Data Cleaning Project 

### 🎯 Overview
This project simulates a **real-world retail data cleaning scenario** for a mid-sized e-commerce company.  
It focuses on transforming messy and inconsistent customer, product, and order data into a fully standardized, analytics-ready dataset.

The project was built in **Google Sheets / Excel** and follows a structured, reproducible data cleaning workflow.

---

### 🗂️ Project Structure
| Sheet Name | Description |
|-------------|-------------|
| `orders_raw`, `customers_raw`, `products_raw` | Original uncleaned data |
| `orders_clean`, `customers_clean` | Cleaned and standardized datasets |
| `products_master_corrected` | Reference table used for validation |
| `KPI` | Data Quality KPIs and summary metrics |
| `tasks_brief` | Analyst task breakdown and project plan |
| `Issue Escalation & Stakeholder` | Simulated project communication log |

---

### ⚙️ Cleaning Process
1. **Raw Data Review:**  
   Identified issues in dates, phone numbers, emails, currencies, SKU mismatches, and missing fields.

2. **Standardization:**  
   Used formula-based cleaning (`TRIM`, `PROPER`, `REGEXREPLACE`, `SUBSTITUTE`, `IFERROR`, `ARRAYFORMULA`)  
   to unify text casing, remove extra spaces, and fix format inconsistencies.

3. **Validation Flags:**  
   Created flag columns (`*_flag`) for each key attribute:  
   - `customer_id_flag`, `email_flag`, `phone_flag`, `sku_flag`, `quantity_flag`, etc.  
   Each flag marks whether the record passes validation ✅ or fails ❌.

4. **Referential Consistency Check:**  
   Ensured that every order links to a valid customer and valid SKU (no orphan records).

5. **KPI Dashboard:**  
   Aggregated all flag results into performance indicators of data quality.

---

### 📊 Data Quality KPIs
| KPI Category | Metric | Result |
|---------------|---------|--------|
| Referential Consistency | Valid SKU & Customer IDs | **100%** |
| Data Completeness | Required Fields Filled | **96.17%** |
| Data Uniqueness | Unique IDs Across Tables | **100%** |
| Data Validity | Correct Formats & Values | **>95%** |

---

### 🧠 Key Learnings
- Building **flag-based validation systems** helps track errors transparently.  
- Maintaining a **separate KPI sheet** quantifies data quality improvements.  
- Even in Excel/Sheets, it's possible to simulate a **full analyst workflow**—from cleaning to reporting.  
- Documentation (brief + stakeholder notes) adds **professional realism** to portfolio projects.

---

### 💾 Tools & Skills Used
- **Google Sheets / Excel**
- Regular Expressions (REGEXMATCH / REGEXREPLACE)
- Logical Formulas (IF, AND, OR, IFERROR)
- Text & Date Standardization (PROPER, TRIM, VALUE)
- Data Quality KPI Metrics
- Documentation for project stakeholders

---

### 🏁 Project Status
✅ Completed – ready for portfolio publication.  
This is **Project** in a retail data cleaning series, demonstrating practical end-to-end data cleaning workflows.

---

**Author:** Damian Sobolewski 
**Year:** 2025  