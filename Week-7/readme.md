# 📊 Power BI Sales Analytics & Campaign Performance Dashboard

## 📁 Project Overview

This project is a complete end-to-end Power BI report designed to analyze **sales performance**, **product pricing strategy**, **customer segmentation**, and **marketing campaign impact** across various regions, dates, and product categories. It incorporates advanced DAX techniques, time intelligence, and licensing documentation for professional deployment scenarios.

---

## 📌 Key Features

- Interactive dashboards with slicers for **Campaign**, **Product**, **Customer**, and **Geo Location**
- Real-time KPIs: Total Sales, Total Profit, Units Sold, Profit Margin, and Average Unit Price
- Campaign-level performance analytics
- Product pricing segmentation using custom logic
- DAX-driven visualizations for:
  - Year-over-Year and Month-over-Month performance
  - High/Low selling products
  - Customer and geo-level contribution
- Embedded DAX functions such as `ALL`, `FILTER`, `ALLSELECTED`, `SELECTEDVALUE`, and more

---

## 🛠️ DAX Techniques Implemented

### Measures:
- `Total Sales`
- `Total Profit`
- `Profit Margin`
- `Avg Unit Price`
- `% Contribution of Product`
- `Sales by Category`, `Sales by Region`

### Context Manipulation using `CALCULATE()`:
- `ALL(Product)` – Remove filters for benchmarking
- `ALLSELECTED(Product)` – Respect slicer selections
- `FILTER(Product, ...)` – Apply custom row filters
- `REMOVEFILTERS(...)` – Clear filter context
- `VALUES(...)` – Unique category logic
- `SELECTEDVALUE(...)` – Dynamic value selection
- `ISFILTERED(...)` – Conditional logic based on user input

---

## 📆 Date Time Functions

- `TODAY()` – Current date evaluation
- `YEAR()`, `MONTH()` – Extract calendar parts
- `DATEADD()` – Calculate previous month/year sales
- `DATEDIFF()` – Time between two events (e.g., signup vs today)
- `EOMONTH()` – End of month identification

---

## 🧠 Advanced Analytics

- Product Segmentation: Premium, Mid-Range, Budget
- RankX-based top product analysis
- Paginated report readiness (for Premium)
- KPI cards, bar charts, line graphs, matrices

---

## 📚 Power BI Licensing Summary

### Types:
- Power BI Free
- Power BI Pro
- Power BI Premium Per User (PPU)
- Power BI Premium (Capacity-Based)
- Power BI Embedded

### Premium Benefits:
- Dedicated capacity
- Larger datasets (up to 400 GB)
- Paginated reporting
- AI & ML features
- Higher refresh limits (48/day)
- Enterprise-scale sharing

_Read the full [Power BI Licensing Documentation](#)_

---

## 📦 Files Included

| File/Folder | Description |
|-------------|-------------|
| `PowerBI_Sales_Report.pbix` | Main Power BI report |
| `README.md` | Project overview |
| `DAX_Measures.txt` | All custom DAX measures used |
| `PowerBI_Licensing_Documentation.pdf` | Summary of licensing models |
| `Data Model Screenshot.png` | Schema reference for all relationships |
| `Campaign_Customer_Geo_Product_Sales.csv` | Input data files (optional if shared externally) |

---

## 🚀 How to Use

1. Open `PowerBI_Sales_Report.pbix` in Power BI Desktop
2. Ensure data connections are valid or rebind with provided data files
3. Explore the dashboard using slicers for date, campaign, customer, etc.
4. Review DAX code by right-clicking on each measure
5. Modify or extend visualizations as per your project needs

---

## 🏁 Future Enhancements

- Add RLS (Row Level Security) for user-based access
- Integrate paginated reports using Premium workspace
- Embed dashboard in a web portal using Power BI Embedded
- Implement real-time streaming dataset

---

## 📞 Contact

For feedback, questions, or collaboration opportunities:

**Raj Awasthi**  
📧 raj.awasthi@email.com  
🌐 [LinkedIn](https://www.linkedin.com/in/raj-awasthi) (example link)

---

