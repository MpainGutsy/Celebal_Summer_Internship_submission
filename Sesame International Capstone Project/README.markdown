# Sesame International Power BI Project

## Introduction

This Power BI project is designed for Sesame International, a company incorporated in 1986 and engaged in the processing and export of hulled sesame seeds. Operating a processing unit in Muzaffarnagar with an installed capacity of 5,500 Metric Tonnes per annum, Sesame International is a 100% export-oriented unit with markets in Germany, France, USA, UK, and China. The project aims to modernize the company’s traditional enterprise reporting by integrating Power BI for interactive dashboards and reports, providing comprehensive financial and operational insights to support decision-making and operational efficiency.

## Project Scope

The project addresses the following reporting and KPI requirements specified by Sesame International’s management:

1. **Tabular View of Profit and Loss (P&L) Accounts and Balance Sheet**:
   - Matrix/table visuals with the ability to add sub-categories to main categories.

2. **Graphical Representation**:
   - Yearly trends of P&L line items with year-on-year growth or degrowth indicators.

3. **Funnel Chart**:
   - Step-by-step visualization of key line items from Gross Sales to Net Profit.

4. **KPI Cards**:
   - Financial ratios for the current year compared with the previous year, including:
     - Operating Profit Margin
     - Net Profit Margin
     - Return on Capital Employed (ROCE)
     - Debt-Equity Ratio
     - Interest Coverage Ratio
     - Debt to Profit Ratio
     - Net Working Capital Intensity
     - Debtor Days
     - Inventory Days
     - Days Payable

5. **Country-wise Sales Visualization**:
   - Sales by year and percentage of total sales for each country.

6. **Top 5 Customers Sales Visualization**:
   - Sales to the top 5 customers by year with percentage of total sales.

7. **Product-wise Sales Visualization**:
   - Sales by product by year with percentage of total sales.

8. **Capacity Utilization Visualization**:
   - Total installed capacity, capacity utilized, and percentage capacity utilized by year.

9. **Additional Visualizations**:
   - Any other visualizations deemed valuable by the developer/analyst, as the management welcomes innovative analysis methods.

## Data Sources

The data for this project is sourced from Sesame International’s internal systems, including:

- **Financial Statements**: Profit and Loss (P&L) accounts and Balance Sheets, providing data on revenues, expenses, assets, liabilities, and equity.
- **Sales Data**: Records of sales segmented by country, customer, and product, reflecting the company’s export markets (Germany, France, USA, UK, China).
- **Production Data**: Information on total installed capacity (5,500 Metric Tonnes per annum) and actual production for capacity utilization calculations.

The data is assumed to be available in formats such as Excel files, CSV files, or a database (e.g., SQL Server) that can be connected to Power BI.

## Data Model

The Power BI data model includes the following tables:

- **Financials**: Contains P&L and Balance Sheet data, including line items such as revenues, expenses, assets, liabilities, and equity.
- **Sales**: Contains sales data segmented by country, customer, product, and year, along with total sales figures.
- **Production**: Contains data on total installed capacity and actual production for each year.

**Relationships**:
- Tables are linked using common keys such as date (for time-based analysis), product, and customer.
- Calculated columns and measures are created in Power BI using DAX (Data Analysis Expressions) to compute financial ratios and other KPIs.

**Example Measures**:
- `Total Sales = SUM(Sales[Sales Amount])`
- `Year-on-Year Growth = (CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date])) - [Total Sales]) / CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))`

## Visualizations

The project includes the following visualizations to meet the specified requirements:

### 1. Tabular View of P&L and Balance Sheet
- **Type**: Matrix/Table
- **Details**: Displays P&L and Balance Sheet data with drill-down capabilities for sub-categories (e.g., breaking down operating expenses into salaries, utilities, etc.).
- **Purpose**: Provides a detailed view of financial statements with interactive filtering.

### 2. Yearly Trend of P&L Line Items
- **Type**: Line Chart
- **Details**: Shows trends of key P&L line items (e.g., Gross Sales, Operating Profit, Net Profit) over multiple years, with annotations or secondary measures for year-on-year growth/degrowth.
- **Purpose**: Highlights financial performance trends over time.

### 3. Income Statement Funnel
- **Type**: Funnel Chart
- **Details**: Visualizes the progression from Gross Sales to Net Profit, showing key stages such as Cost of Goods Sold, Operating Expenses, and Taxes.
- **Purpose**: Illustrates the flow of revenue to profit, identifying areas of significant impact.

### 4. KPI Cards for Financial Ratios
- **Type**: Card
- **Details**: Each card displays a specific financial ratio (e.g., Operating Profit Margin, Net Profit Margin) with current-year and previous-year values for comparison.
- **Purpose**: Provides a quick snapshot of financial health and performance.

### 5. Country-wise Sales
- **Type**: Stacked Bar Chart or Map
- **Details**: Shows sales by country (Germany, France, USA, UK, China) over years, with percentages of total sales displayed.
- **Purpose**: Highlights geographic sales distribution and trends.

### 6. Top 5 Customers Sales
- **Type**: Clustered Column Chart
- **Details**: Displays sales to the top 5 customers by year, including the percentage of total sales for each.
- **Purpose**: Identifies key customers contributing to revenue.

### 7. Product-wise Sales
- **Type**: Stacked Column Chart
- **Details**: Shows sales by product over years, with percentages of total sales for each product.
- **Purpose**: Analyzes product performance and contribution to revenue.

### 8. Capacity Utilization
- **Type**: Line Chart or Gauge
- **Details**: Visualizes total installed capacity (5,500 Metric Tonnes), capacity utilized, and percentage capacity utilized by year (% capacity utilized = Capacity Utilized / Total Capacity).
- **Purpose**: Monitors production efficiency and capacity usage.

### 9. Additional Visualizations
- **Type**: Developer’s discretion (e.g., Pie Chart, Area Chart, or Scatter Plot)
- **Details**: Potential additions include:
  - A pie chart showing the proportion of sales by country.
  - A trend analysis of raw material costs.
  - A scatter plot comparing profitability across products.
- **Purpose**: Enhances insights by exploring additional data relationships.

## KPIs

The following financial ratios and KPIs are calculated and visualized using DAX measures in Power BI:

| S. No. | Ratio                      | Formula                                                                 |
|--------|----------------------------|-------------------------------------------------------------------------|
| 1      | Operating Profit Margin    | OPBDITA / Operating Income                                              |
| 2      | Net Profit Margin          | PAT / Operating Income                                                 |
| 3      | Return on Capital Employed (ROCE) | EBIT / Capital Employed (Capital Employed = Total Assets – Current Liabilities) |
| 4      | Debt-Equity Ratio          | Total Debt / Total Equity (Total Equity = Tangible Net Worth + Minority Interest) |
| 5      | Interest Coverage Ratio    | OPBDITA / Interest and Finance Charges                                  |
| 6      | Debt to Profit Ratio       | Total Debt / OPBDITA                                                   |
| 7      | Net Working Capital Intensity | Net Working Capital / Operating Income (NWC = Total Current Assets – Cash and Bank Balances – (Trade Creditors + Advances from Customers + Income Taxes Payable + Other Operating Current Liabilities and Provision)) |
| 8      | Debtor Days                | Accounts Receivable * 365 / (Gross Sales + Traded Goods Sales)         |
| 9      | Inventory Days             | Total Inventory * 365 / Total Cost of Manufacturing                    |
| 10     | Days Payable               | Trade Creditors / (Raw Material Consumption + Traded Goods Purchased + Consumable Stores + Power and Fuel + Employee Costs + Other Manufacturing Expenses) |

These KPIs are displayed using KPI cards, allowing users to quickly assess financial performance and compare metrics across years.

## How to Use

- **Data Refresh**:
  - If connected to a live data source (e.g., a SQL database or cloud storage), users can refresh the data by clicking the “Refresh” button in Power BI Desktop or the Power BI Service.
  - Ensure the data source connections are properly configured with the correct credentials.

- **Navigation**:
  - The report is organized into multiple pages, each focusing on a specific aspect (e.g., Financials, Sales, Capacity Utilization).
  - Use the page navigation controls in Power BI to switch between pages.

- **Interactivity**:
  - Slicers and filters are included to allow users to filter data by year, country, customer, or product.
  - Drill-down features in matrix visuals enable exploration of sub-categories in financial statements.

## Future Enhancements

Sesame International’s management welcomes new ideas and analysis methods. Potential enhancements to the Power BI project include:

- **Forecasting**: Implementing predictive analytics to forecast future sales, profits, or capacity utilization based on historical trends.
- **Cost Analysis**: Detailed breakdown of raw material costs (sourced from Gujarat, Madhya Pradesh, Uttar Pradesh, and Rajasthan) and their impact on profitability.
- **Industry Benchmarking**: Comparing Sesame International’s financial ratios and operational metrics with industry benchmarks to assess competitive performance.
- **Drill-Through Reports**: Adding drill-through pages for transaction-level details, such as individual customer sales or specific production batches.
- **Raw Material Price Trends**: Visualizing price appreciation trends for natural sesame seeds to inform purchasing strategies.

## Technical Notes

- **Power BI Version**: The project is compatible with the latest version of Power BI Desktop (as of July 2025). Ensure you are using an up-to-date version for optimal performance.
- **Custom DAX Formulas**: The project includes custom DAX measures for calculating financial ratios, year-on-year growth, and other KPIs. Example:
  - `Operating Profit Margin = DIVIDE([OPBDITA], [Operating Income], 0)`
  - `Debtor Days = [Accounts Receivable] * 365 / ([Gross Sales] + [Traded Goods Sales])`
- **Project Structure**: The Power BI project follows best practices, with separate folders for the semantic model (`<project name>.SemanticModel/`) and report (`<project name>.Report/`) if saved as a Power BI Project (PBIP) file.
- **Version Control**: The project is designed for compatibility with Git for version control, enabling collaboration and tracking of changes.
- **Data Connectivity**: Ensure proper configuration of data source connections, especially if using cloud-based sources like Azure SQL Database or SharePoint.
- **Limitations**:
  - External changes to project files (e.g., via Visual Studio Code) require restarting Power BI Desktop to reflect updates.
  - Ensure project file paths do not exceed 260 characters to avoid issues on Windows systems.
  - Avoid saving directly to OneDrive/SharePoint; use locally synced folders to prevent syncing issues.

## Contact and Support

For questions or support regarding the Power BI project, contact the development team or refer to the [Power BI Community](https://community.powerbi.com/) for additional resources. Feedback and suggestions for new visualizations or analyses are welcome, aligning with Sesame International’s openness to innovative ideas.