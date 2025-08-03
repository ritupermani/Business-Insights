# Business Insights 360 – AtliQ Hardware

🚀 **Comprehensive Business Intelligence Solution using SQL & Power BI**

## 📊 Project Overview

**Business Insights 360** is a real-industry data analytics project built for **AtliQ Hardware**, a multinational hardware manufacturing company that Sells and Manufactures Hardware. They have Customers all over the world and Products under various categories. The goal of this project was to uncover business-critical insights across **Finance**, **Sales**, **Marketing**, and **Supply Chain** domains using SQL and Power BI.

---

## 🛠 Tech Stack

- **Power BI** – Dashboards, DAX, KPI visualization, filters/slicers  
- **Power Query** – Data cleaning and shaping  
- **Excel** – Preliminary analysis and data validation  
- **Data Modeling** – Snowflake schema architecture  
- **DAX studio** – for optimizing the report  

---

## 📘 Power BI Techniques Learnt

- What are all the questions should be asked before starting the project  
- Creating calculated columns  
- Creating measures using DAX language  
- Data modeling  
- Using Bookmarks to switch between two visuals  
- Page navigation with buttons  
- Using DIVIDE function to prevent zero division errors  
- Creating date table using M language  
- Dynamic titles based on the applied filters  
- Using KPI indicators  
- Conditional formatting values using icons/background colors  
- Data validation techniques  
- Power BI services, publishing reports, auto-refresh setup via gateway  
- Power BI App creation  
- Collaboration, workspace, access permissions in Power BI services  

---

## 📚 Business Related Terms

- Gross price  
- Pre-invoice deductions  
- Post-Invoice deductions  
- Net Invoice sale  
- Gross Margin  
- Net sales  
- Net profit  
- COGS - Cost of Goods Sold  
- YTD - Year to Date  
- YTG - Year to Go  
- Direct  
- Retailer  
- Distributors  
- Consumer  

---

## 🧠 Key Features

### 📈 Power BI Dashboard

- Built a dynamic dashboard showcasing Net Sales, Operating Profit, Conversion Rates, and Market Coverage  
- Enabled interactivity with slicers for region, product category, and customer segmentation  
- Applied advanced DAX for KPI indicators and trend analysis  

### 🧩 Data Modeling

- Structured a robust Snowflake schema with fact and dimension tables (e.g., `dim_date`, `dim_product`, `fact_sales`)  
- Ensured optimized performance and flexibility for reporting  

### 📌 Insights Delivered

- Identified underperforming regions and product lines  
- Analyzed campaign effectiveness through conversion rates and customer feedback  
- Provided strategic recommendations for marketing ROI improvement and inventory optimization  

---

## 🗃️ Dataset Understanding

Understanding what data is available will be more helpful while doing analysis. Before jumping on to the analysis, get good understanding of what data is available.

### Dimension Tables  
Static data like details of customer and products

### Fact Tables  
Transactional data  

#### gdb041:
- `dim_customer`  
  - 27 distinct markets (e.g., India, USA, Spain)  
  - 75 customers  
  - 2 platforms: Brick & Mortar, E-commerce  
  - Channels: Retailer, Direct, Distributors  
- `dim_market`  
  - 27 markets, 7 sub-zones, 4 regions (APAC, EU, LATAM, nan)  
- `dim_product`  
  - Divisions: P&A (Peripherals, Accessories), PC (Notebook, Desktop), N&S (Networking, Storage)  
  - 14 categories like Internal HDD, keyboard  
  - Variants per product  
- `fact_forecast_monthly`  
  - Forecasts customer needs for inventory planning  
  - Denormalized by data engineering team for analytics  
- `fact_sales_monthly`  
  - Similar to forecast table but with actual sold quantity  

#### gdb056:
- `freight_cost` – Travel & logistics cost per market/year  
- `gross_price` – Product pricing data  
- `manufacturing_cost` – Manufacturing cost per product/year  
- `pre_invoice_deductions` – Pre-invoice deductions %  
- `post_invoice_deductions` – Post-invoice deductions & others  

---

## 🔌 Importing Data into Power BI

- The database is hosted on **MySQL**
- Connect to MySQL from Power BI using credentials and import tables  

---

## 🧱 Data Model

- Data modeling is the foundation of any report  
- Followed good practices & implemented **Snowflake schema**



![Data Model](https://github.com/ArunGuptaaa/Business-Insights/blob/main/Reports/Data%20Model.png)

---

## 📊 Detailed Dashboards Overview

### 🏠 Home View

Buttons to navigate to each report section:  
- Info  
- Finance View  
- Sales View  
- Marketing View  
- Supply Chain View  
- Executive View  
- Support  

[<img src= "https://github.com/ArunGuptaaa/Business-Insights/blob/main/Reports/Home%20View.png">](https://app.powerbi.com/view?r=eyJrIjoiMTVhODQ3M2UtY2U4Yy00MTNlLWE1YjktN2EwOTkxZmJhMjc2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

> Click the image above to explore the **interactive Power BI dashboard** live.

---

### 💰 Finance View

- Profit & Loss metrics from Gross Sales to Net Profit  
- Benchmarks (LY or Target) selectable through slicers  
- KPIs: Net Sales, Gross Margin %, Net Profit %  
- Performance trend with dynamic comparison  
- Top/Bottom products & customers by Net Sales  

![Finance](https://github.com/ArunGuptaaa/Business-Insights/blob/main/Reports/Finance%20View.png)

---

### 📦 Sales View

- Unit Economics: Sales vs Discounts (Pre & Post Invoice)  
- COGS analysis leading to Gross Margin  
- Customer/Product performance via Net Sales, GM%  
- Market/Customer/Region performance matrix  
- Tooltip trend per customer  

![Sales](https://github.com/ArunGuptaaa/Business-Insights/blob/main/Reports/Sales%20View.png)

---

### 📣 Marketing View

- Net Profit derived after subtracting operational expenses  
- Toggle between:
  - Net Sales & Net Profit %
  - Net Sales & Gross Margin %  
- Matrix view for Segment, Category, and Product performance  

![Marketing](https://github.com/ArunGuptaaa/Business-Insights/blob/main/Reports/Marketing%20View.png)

---

### 🏭 Supply Chain View

- KPIs: Forecast Accuracy, Net Error, Absolute Error  
- Risk factor and net error trend  
- Product and Customer metrics: FA%, LY, Error%, Risk  

![Supply Chain](https://github.com/ArunGuptaaa/Business-Insights/blob/main/Reports/Supply%20Chain%20View.png)

---

### 👑 Executive View

- High-level dashboard for C-Suite  
- Market Share trend (AtliQ vs Competitors)  
- Revenue by Division and Channel  
- Top 5 Products & Customers  
- Sub-Zone insights with Revenue %  

![Executive](https://github.com/ArunGuptaaa/Business-Insights/blob/main/Reports/Executive%20View.png)

---

## 🧠 Key Learnings

- Most helpful KPIs for C-level: **Gross Margin** & **Net Profit**  
- Sales teams focus more on **Net Sales** & **Gross Margin**  
- For marketing: Track **Spend vs Revenue** and impact on Gross Margin  
- Supply chain: **Forecast Accuracy**, **Net/Abs Error**, **Risk**  
- One of the most important skills: **Stakeholder expectation management**

📁 **Download Report**: [business_insights_360](https://github.com/ArunGuptaaa/Business-Insights/blob/main/business_insights_360.pbix)

---

## 📌 Conclusion

This project showcases how SQL and Power BI can work together to build a data-driven decision support system. From database design to BI dashboarding, Business Insights 360 covers the full analytics lifecycle for enterprise-scale insights.

---

⭐ If you found this project insightful, feel free to star the repo or connect!
