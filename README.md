# PulseSales: Sales & Revenue Analysis Dashboard
PulseSales is a premium, highly interactive, and responsive web dashboard designed to analyze and visualize sales data. It features responsive sidebars for CSV and Excel file imports, slice-and-dice filters, live KPI tracking, multi-axis visual charts, automated business insights, and a raw data explorer table.
This project is built using pure **HTML5**, **Vanilla CSS**, and **ES6+ JavaScript**, leveraging modern client-side library CDNs (Chart.js, PapaParse, SheetJS, and Lucide Icons). Because it is fully static, you can deploy it to **GitHub Pages** for free with zero server configurations.
---
## Key Features
1. **Robust Data Import**:
   - Drag-and-drop or browse files to load **CSV** spreadsheets (parsed via `PapaParse`).
   - Import **Excel (`.xlsx`, `.xls`)** sheets (read via `SheetJS`).
   - One-click **Demo Data Loader** pre-populated with supermarket sales transactions matching the standard Kaggle supermarket schema.
   - Dynamic schema mapping that auto-detects and sanitizes column headers (e.g. mapping "Sales", "Revenue", or "Total" to the primary currency metric).
2. **Executive KPI Cards**:
   - **Total Revenue**: Cumulative sum of overall transaction values.
   - **Sales Volume**: Overall count of individual items sold.
   - **Customer Satisfaction**: Overall customer rating averages (out of 10.0).
   - **Gross Profit Margin**: Dynamic calculations comparing transaction value to the cost of goods sold (`COGS`).
   - **Period-over-Period Sparkline Trends**: Automatically bisects the filtered timeframe to calculate growth differentials (e.g. `+12.4% vs early period`).
3. **Multi-Axis Interactive Visualizations (Chart.js)**:
   - **Revenue Trend**: Visual line graph of aggregated daily or weekly revenue.
   - **Sales by Product Line**: Grouped horizontal bar chart sorting departments by performance.
   - **Branch Performance**: Combo bar (revenue) + line (avg satisfaction score) chart highlighting branch operational metrics.
   - **Distribution Splits**: Toggleable donut charts analyzing sales breakdown by payment methods or customer segments.
4. **Automated Business Insights**:
   - Generates natural language analysis cards on-the-fly based on current filter states, evaluating:
     - Top revenue-generating categories and their total revenue shares.
     - Customer satisfaction leaders (Branches/Cities with top ratings).
     - Loyalty program impact (average spend of members vs. walk-in customers).
     - Operational peaks (the day of the week generating the highest sales).
5. **Raw Data Explorer**:
   - Clean, scrollable database viewer containing loaded invoices.
   - Instant search filters indexing Invoice ID, Branch, Category, City, or Payment method.
   - Interactive table header clicks for column-based ascending or descending sorting.
   - Custom paginator with page-size controllers (5, 10, 25, 50 rows).
6. **Interactive Styling & Theming**:
   - Fluid responsive layout adapting to Desktop, Tablet, and Mobile screens.
   - Dynamic Dark / Light theme switcher with local storage persistence.
   - Modern glassmorphism card designs with hover micro-animations.

