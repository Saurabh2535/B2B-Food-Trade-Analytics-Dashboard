# B2B-Food-Trade-Analytics-Dashboard


## 📊 Project Overview

This repository features an Excel analytics dashboard for a simulated B2B food trade dataset, inspired workflow and data-driven business practices in cross-border agri-exports. The project demonstrates end-to-end data cleaning, preprocessing, KPI engineering, and dashboard design for business intelligence and operations insight.

---

## 🗃️ Dataset

- **Size:** 50,000 rows × 15 columns (Order-level data)
- **Key Columns:**  
  `Order_ID, Product, Supplier, Customer, Quantity_MT, Price_per_MT_USD, Total_Value_USD, Order_Date, Delivery_Date, Delivery_Delay_Days, Region, Port, State, Return_Status, Payment_Status`
- **Added Helper Columns:**  
  - `Order_Month` — Extracted month for trend analysis  
  - `Delivery_Status` — "Delayed"/"OnTime" (threshold customizable)  
  - `Payment_Flag`, `Return_Flag` — Binary (1/0) for paid/returned orders

---

## 🛠️ Process & Features

### 1. Data Cleaning & Preprocessing
- **Formatted as Excel Table** for robust referencing *(TradeData)*
- Ensured **no duplicates** or blanks in critical columns
- Standardized all categorical fields (e.g., Payment_Status, Return_Status)
- **Sanity checks** on numeric fields (no negative/zero Quantity or Delay)
- Created binary flags and helper columns for efficient KPI analysis

### 2. Pivot Table Analytics
- **KPI Pivots:**  
  - Total Orders (Order_ID, count)  
  - Total Sales (Total_Value_USD, sum)  
  - Average Delay (Delivery_Delay_Days, avg)
  - **% Paid Orders / % Returned Orders:**  
    - Calculated via `GETPIVOTDATA()` to ensure slicer interactivity
- **Other analytics:**  
  - Monthly Trends
  - Product/State Leaders
  - Return/Payment Status rates

### 3. Dashboard Design
- **KPI Cards:** Big-number flash for main metrics (top row)
- **Charts/Visualizations:**  
  - Monthly line trend  
  - Top 10 products (bar)  
  - Orders by state (bar)  
  - Payment & return rates (donut/pie)  
  - Delivery delays (line, segmented)
- **Slicers for interactivity:**  
  - Product, State, Port, Month, Payment Status  
  - All visuals update dynamically

---

## 🌟 Sample Key Insights

- **Monthly Trends:** January sees the highest orders (seasonality confirmed)
- **Product Leader:** Cashew is the top-selling export
- **Return Rate:** 25% returned, 75% not returned (potential process issue)
- **State Leader:** Gujarat has the highest export volume
- **Payment Status:** 75% paid, 25% unpaid
- **Delivery:** Highest delay found in West Bengal, June (9.34 days avg)

---

## 📷 Dashboard Screenshot

<img width="1312" height="440" alt="Screenshot (1869)" src="https://github.com/user-attachments/assets/f0c72eae-6119-4a5d-95d9-c4f4a2fbca26" />


---

## 🚀 How to Use

1. Open `ProSessedAI_FoodTrade_Analytics_2024.xlsx` in Microsoft Excel.
2. Go to the `Dashboard` sheet for main insights and interactivity.
3. Use the slicers (Product, State, Port, Month, Payment Status) to drill down KPIs and charts by different segments.

---

## 🧑‍💻 Skills Demonstrated

- Data cleaning & preprocessing (Excel formulas, Table design)
- Advanced PivotTables & formula engineering (GETPIVOTDATA)
- Dashboard & data visualization best practices
- Deriving actionable business insights from large data
- Professional documentation and self-service analytics

---

## 👤 Author

- **Saurabh S Acharya**
- https://www.linkedin.com/in/saurabhsacharya/
---

**If you like the project, star ⭐ the repo or get in touch!**

