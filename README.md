# 🏠 Housing Market Analysis with Google BigQuery & Power BI

### 🔹 1. Overview  
![Overview](./assets/Dashboards/Overview.png)

---

### 🔹 2. Top & Bottom 5 Products by Sales, Profit, Quantity Sold  
![Top and Bottom 5 Analysis](./assets/Dashboards/Top%20and%20Bottom%205%20Sales%20Profit%20Quantity%20Analysis.png)

---

### 🔹 3. Comparison of Sales, Profit & Quantity Between Two Time Periods  
![Comparison](./assets/Dashboards/Comparison%20Sales%20Profit%20Qunality.png)

---

### 🔹 4. Order-Level Table with Filters (Date, Customer, Product, Promotion)  
![Table Visuals](./assets/Dashboards/Table%20Visuals.png)

## 📌 Project Overview
This project analyzes Denmark's housing market using real estate sales data. Leveraging **Google BigQuery** for cloud-based SQL querying and **Power BI** for interactive dashboards, the project offers key insights into trends such as median sales price change, YOY sales growth, and regional housing patterns. This end-to-end data analytics pipeline includes data extraction, transformation, DAX-based modeling, and dashboard deployment.

---

## 🎯 Objectives
- Analyze house sale trends across regions and sales types.
- Understand the impact of time, region, house type, and market factors (interest, inflation, yield) on sales price.
- Build a comprehensive Power BI dashboard to visualize metrics like units sold, sales growth, SQM price, and performance KPIs.

---

## 🧰 Tools & Technologies
- **Google BigQuery** (Cloud SQL querying)
- **Microsoft Power BI** (Data modeling & visualization)
- **Power Query Editor** (Data cleaning)
- **DAX (Data Analysis Expressions)**

---

## 🗂️ Dataset
- **Source**: Imported into **Google BigQuery**
- **Structure**: Includes fields such as `region`, `sales_type`, `house_type`, `purchase_price`, `offer_price`, `area_sqm`, `interest`, `inflation`, `yield`, `date`

---

## 🔄 Workflow

### 1. Data Loading
- Set up a **free Google Cloud account**
- Load real estate data into **Google BigQuery**
- Connect BigQuery with **Power BI Desktop**

### 2. Data Exploration & Cleaning
- Used **SQL in BigQuery** to preview and understand the dataset
- Cleaned and transformed data using **Power Query Editor**

### 3. DAX Measures & Analysis
- **YOY Sales Growth** using `CALCULATE`, `MAX`, `YEAR`, `IF`, `BLANK`
- **Offer vs Purchase Price** scatter plots
- **Median Price Change** by region using `MEDIANX`
- **Units Sold by Year/Quarter** with `DISTINCTCOUNT` and `CALCULATE`
- **Last 12 Months Sales** with `DATESINPERIOD`, `CALCULATE`, `SUM`
- **Sales Performance** and **Sales by Region** using `ALLEXCEPT`, `TOTALYTD`
- **Offer to SQM Price** and **Age column** for Key Influencers visual
- **Comparison visuals** like Avg Offer/Purchase Price by House Type and Avg Inflation/Interest/Yield

### 4. Dashboard Publishing
- Published interactive report to **Power BI Service**
- Created a new **Workspace**, added clustered bar charts and visuals for house type analysis

---

## 📊 Key Insights

- **YOY Growth**: Auction sales showed the highest positive growth (+0.29), while regular and family sales types showed decline.
- **Purchase vs Offer Price**: Most properties were purchased at or slightly below offer price.
- **Regional Trends**:
  - **Zealand** led in total sales (95bn DKK)
  - **Bornholm** had the lowest average SQM price.
- **Sales Performance**: Peaked in 1992 Q1 and varied by region and house type.
- **Key Influencers**: Age and property size significantly influenced purchase price.

---

## 📁 Project Structure
