# Infinity Tech Expense Tracker 🧾

## 📌 Overview
This Excel-based dashboard is designed to help companies like *Infinity Tech* track and analyze their expenses efficiently. It enables stakeholders to gain insights into expense patterns, vendor reliance, departmental spend, and more—all in a clean, interactive format.

## 🧠 Features
- Capital vs Operational Expense Analysis
- Quarterly and Monthly Trends
- Expense breakdown by:
  - Department
  - Vendor
  - Payment Method
  - Nature (CapEx / OpEx)
- PO Usage Insights
- Slicers for real-time filtering
- Clean KPI cards with dynamic value linking

## ⚙️ KPI Formulas
| KPI | Formula |
|-----|---------|
| Total Expenses | `=SUMIFS(Table1[Amount], ...)` |
| CapEx Total | `=SUMIFS(Table1[Amount], Table1[Nature], "Capital")` |
| OpEx Total | `=SUMIFS(Table1[Amount], Table1[Nature], "Operational")` |
| Highest Spending Vendor | `=INDEX(...)` with `MAX` |
| PO Usage % | `=COUNTIFS(...)/COUNT(...)` |
| Total Departments | `=COUNTA(UNIQUE(...))` |

## 💡 Number Formatting Used
- Millions: `###.0,,\M`
- Thousands: `###.0,\K`

## 📂 File Structure
- `Corporate_Budget_Tracker.xlsx`: Contains all pivot tables, KPI cards, slicers, and final dashboard in the "Dashboard" sheet.

## 🎯 Use Cases
- Financial Planning
- Budget Reviews
- Vendor Cost Analysis
- Expense Reporting 

## Dashboard Screenshort
![Infinity Tech Expense Tracker Dashboard](https://raw.githubusercontent.com/Bheki0987/Infinity-Tech-Expense-Tracker/main/images/Dashboard-Screenshot.png)


## 🧑‍💼 Author
**Bheki Mogola**  
Aspiring Data Analyst | Excel + Tableau + SQL + Python  
[LinkedIn](https://www.linkedin.com/in/bheki-mogola-8481122b7)

---

