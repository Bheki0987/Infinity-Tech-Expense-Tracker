# Infinity Tech Expense Tracker 🧾

## 📌 Overview
This Excel-based dashboard is designed to help *Infinity Tech* track and analyze their expenses efficiently. It enables stakeholders to gain insights into expense patterns, vendor reliance, departmental spend, and more—all in a clean, interactive format.

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
![Infinity Tech Expense Tracker Dashboard](https://raw.githubusercontent.com/Bheki0987/Infinity-Tech-Expense-Tracker/main/Dashboard-Screenshot.png)

## Findings
- Total & Breakdown of Expenses
  - Total recorded expenses: R1.3M
  - Split almost evenly between Capital (R646.1K, 49.7%) and Operational (R615.5K, 47.3%) expenditures.
  - Capital spending slightly exceeds operational, highlighting investment-heavy cost allocation.

- Departmental Insights
  - Training & Development is the highest-spending department with ~R177K.
  - Other high spenders include IT Infrastructure (R154K) and Admin & Operations (~R143K).
  - HR and Marketing have the lowest spend (<R100K), suggesting leaner operations.
  
- Vendor Analysis
  - Expenses are concentrated among a few vendors:
    - Vendor D: R268.9K (highest).
    - Vendor E: R261.5K.
    - Vendor B: R257.1K.
  - Vendor concentration risk exists since 3 vendors account for over 60% of total vendor expenses.

- Nature of Expenses
  - Non-Essential expenses (53%) outweigh Essential (47%), raising questions about budget efficiency.
  - Opportunity exists to optimize discretionary/non-essential spending.

- Quarterly Expense Trends
  - Q1: R297.7K → gradual increase → Q4: R326.1K.
  - This indicates steady expense growth, possibly linked to project expansions or inflationary pressures.
  - Spike in July 2023 (high-expense month) needs further breakdown to identify drivers.

- Purchase Orders (PO) Usage
  - High PO usage observed (R7.8K – R4.9K range across POs).
  - Consistent spend pattern suggests controlled procurement, though some larger POs stand out.

## 🔎 Business Implications
- Cost Optimization: Non-essential spend > essential → tighten control to reallocate funds toward strategic priorities.
- Vendor Dependency Risk: Heavy reliance on 3 vendors could impact pricing and negotiation leverage.
- Training & Development Spend: While positive for employee growth, at >13% of total expenses, management must evaluate ROI.
- Expense Growth: Continuous quarterly increases highlight need for budget forecasting and variance analysis.

## 🧑‍💼 Author
**Bheki Mogola**  
Aspiring Data Analyst | Excel + Tableau + SQL + Python  
[LinkedIn](https://www.linkedin.com/in/bheki-mogola-8481122b7)

---

