# 📁 Week 1 Submission – Power BI Project

## 📌 Overview

This week’s submission covers the **end-to-end process of data extraction, transformation, loading (ETL)** and analysis of multiple datasets using **Power BI**. The goal was to generate **meaningful business insights** by leveraging Power BI’s modeling capabilities, visuals, and DAX functions.

---

## ✅ Key Activities

### 1. 🔄 Data Extraction & Loading

- Imported datasets from multiple sources including `.csv`, Excel, and web.
- Used **Power Query** for:
  - Data type conversion
  - Removing nulls and duplicates
  - Standardizing column names and formats
  - Merging and appending related datasets

### 2. 🧱 Data Model Creation

- Established relationships between tables (1-to-many, many-to-one)
- Built a **star schema** using fact and dimension tables:
  - **Fact Table:** Sales
  - **Dimension Tables:** Date, Product, Geo, Customer, Campaign

### 3. 📊 Analysis & Insights

Utilized Power BI to explore trends, patterns, and key KPIs:

- **Sales by Region**: Identified top-performing locations using map visuals
- **Revenue Trends**: Analyzed monthly and quarterly revenue patterns
- **Customer Segmentation**: Grouped customers by purchase volume and frequency
- **Product Performance**: Compared units sold and profitability across categories
- **Campaign Impact**: Evaluated campaign-wise contribution to sales

### 4. 🧠 DAX Measures & Functions Used

- Created over 15 calculated **measures** and **columns** using:
  - `CALCULATE()`, `FILTER()`, `ALL()`, `REMOVEFILTERS()`, `SELECTEDVALUE()`
  - `SUMX()`, `DIVIDE()`, `RANKX()`, `SWITCH()`, `IF()`
  - Time intelligence functions: `TOTALYTD()`, `DATEADD()`, `EOMONTH()`

### 5. 📈 Power BI Visuals Applied

- **Card Visuals** for KPIs (Total Sales, Profit Margin, etc.)
- **Line & Bar Charts** for trend analysis
- **Matrix/Table Views** for detailed breakdowns
- **Slicers & Filters** for dynamic user interaction
- **Map Visual** for geo-based insights

---

## 📎 Insights Generated

- Identified underperforming regions and top growth markets
- Found correlation between product pricing and customer retention
- Quantified the impact of marketing campaigns on sales uplift
- Highlighted sales seasonality trends using date hierarchies

---

## 🧰 Tools & Technologies

- **Power BI Desktop**
- **Power Query Editor**
- **DAX (Data Analysis Expressions)**
- Excel & CSV data sources

---

## 📅 Timeline

- **Week 1 Focus:** ETL + Base model + Initial dashboards
- **Next Steps (Week 2):** Advanced KPIs, drillthrough reports, tooltips, bookmarks, and publishing to Power BI Service

---

## 📝 Conclusion

The Week 1 submission demonstrates strong foundations in building a complete Power BI workflow—from raw data to actionable insights. The project showcases the ability to create clean data models, use advanced DAX, and visualize business metrics effectively.

