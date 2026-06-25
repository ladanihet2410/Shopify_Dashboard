# 🛒 Shopify | Sales & Customer Funnel Report — Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-orange)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-blue)
![Excel](https://img.shields.io/badge/Data-Excel-217346?logo=microsoftexcel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

> **Tool:** Microsoft Power BI &nbsp;|&nbsp; **Domain:** E-Commerce Sales & Customer Analytics  
> **Author:** Het Ladani

---

## 📌 About This Project

An end-to-end **Power BI analytics dashboard** built to analyze Shopify sales data and uncover meaningful insights into **transaction performance**, **customer purchasing behavior**, and **long-term customer value**. The dashboard helps stakeholders identify patterns in revenue generation, customer retention, payment methods, and product trends — enabling data-driven decision-making across sales and marketing.

---

## 📂 Repository Structure

```
Shopify_Dashboard/
│
├── 📊 Overview.png                      ← Screenshot of the main Sales & Customer Funnel dashboard
├── 📋 Detailed_Analysis.png             ← Screenshot of the drill-through transaction records page
├── 📁 Shopify Sales.xlsx                ← Raw dataset used to build the dashboard
└── 🖼️ shopify-logo-png-transparent.png  ← Shopify logo asset used in the dashboard design
```

> 💡 **Quick navigation:**
> - Want to see the main dashboard? → [`Overview.png`](./Overview.png)
> - Want to see the detailed records page? → [`Detailed_Analysis.png`](./Detailed_Analysis.png)
> - Want the raw data? → [`Shopify Sales.xlsx`](./Shopify%20Sales.xlsx)

---

## 🖥️ Dashboard Pages

### Page 1 — Shopify Analysis (Overview Dashboard)

> 📸 **Screenshot:** [`Overview.png`](./Overview.png)

The main summary page covering all KPIs, regional insights, trends, and product/payment breakdowns.

#### 📦 Transaction Performance KPIs

| Metric | Value |
|--------|-------|
| 💰 Net Sales | $41,80,874 |
| 📦 Total Quantity | 7,534 |
| 🧾 Net Avg Order Value | $562.6 |

#### 👥 Customer Purchase Behavior KPIs

| Metric | Value |
|--------|-------|
| 👤 Total Customers | 4,431 |
| 🔂 Single Order Customers | 2,392 |
| 🔁 Repeat Customers | 2,039 |

#### 🔒 Retention & Value KPIs

| Metric | Value |
|--------|-------|
| 💎 Lifetime Value (LTV) | $943.6 |
| 🔄 Repeat Rate | 46% |
| 🛒 Purchase Frequency | 1.68 |

#### 📊 Visuals Included

- **Net Sales Trend Over Time** *(Area + Bar Chart)* — Daily and hourly trend of net sales, showing peak activity periods across days and hours
- **Regional Overview – Cities by Net Sales** *(Bubble Map + Bar Chart)* — US bubble map showing geographic density of sales; bar chart ranking top cities: Washington, Houston, New York City, El Paso, Dallas leading performance
- **Net Sales by Gateway Payment Method** *(Donut Chart)* — Shopify Payments dominates at 58.45% ($24.43M), followed by Amazon Payments (17.62%), PayPal (16.29%), and Gift Card (5.66%)
- **Net Sales by Product Type** *(Bar Chart)* — Running Shoes lead at $1.47M, followed by Tennis Shoes ($0.88M), Walking Shoes ($0.63M), Cycling Shoes ($0.48M), Climbing Shoes ($0.34M), and others

#### 🎛️ Filters & Slicers

| Filter | Options |
|--------|---------|
| **Select Measure** | Net Sales / Total Quantity / Total Customers / Repeat Customers |
| **Gateway** | All / Shopify Payments / PayPal / Gift Card / Amazon Payments / Manual |
| **Province** | All US Provinces |

---

### Page 2 — Details Tab (Drill-Through Records)

> 📸 **Screenshot:** [`Detailed_Analysis.png`](./Detailed_Analysis.png)

A fully scrollable transaction-level data table for granular investigation of individual orders.

**Columns:** Order Number, Customer Name, CID, Province, City, Zip Code, Product Type, Gateway, Net Sales, Total Tax, Total Price USD

**Summary Totals visible at bottom:**
- Total CID Count: **4,296**
- Total Net Sales: **$24,43,740**
- Total Tax: **2,44,374.04**
- Total Price USD: **26,88,114.43**

Use this page to:
- Drill through from any summary visual to see underlying records
- Investigate individual orders, customer locations, and product types
- Validate aggregated KPIs with raw transaction data
- Support compliance checks and audit trails

---

## 🔍 Interactive Features

| Feature | Description |
|---------|-------------|
| **Measure Selector** | Dynamically switches all map, bar chart, and trend visuals between Net Sales, Total Quantity, Total Customers, and Repeat Customers |
| **Gateway Filter** | Filters entire dashboard by payment method — all KPIs and charts update in real time |
| **Province Filter** | Narrows analysis to a specific US state across all visuals |
| **Cross-Visual Filtering** | Clicking any chart element instantly cross-filters all other visuals on the page |
| **Drill-Through Navigation** | Right-click any chart or KPI → navigate to the Details Tab for record-level data |
| **Back Navigation** | Arrow (←) on Details Tab returns seamlessly to the Overview page |

---

## ⚙️ Project Build Steps

The dashboard was built following a structured end-to-end BI workflow:

1. **Requirement Gathering** — Defined KPIs and chart requirements for transaction, customer, and retention analysis
2. **Data Walkthrough** — Explored dataset structure, columns, and data types
3. **Data Connection** — Connected Power BI to the Shopify Sales Excel dataset
4. **Data Cleaning / Quality Check** — Handled nulls, standardized formats, and validated data
5. **Data Modeling** — Built relational schema and defined table relationships
6. **Data Processing** — Transformed data using Power Query (ETL)
7. **DAX Calculations** — Created measures for Net Sales, LTV, Repeat Rate, Purchase Frequency, Avg Order Value, and more
8. **Dashboard Layouting** — Designed the dark-themed page structure with navigation panel
9. **Charts Development** — Built and formatted all visuals with dynamic measure selectors
10. **Dashboard Development** — Final assembly of Overview and Details pages with full interactivity
11. **Insights Generation** — Extracted actionable business findings from completed dashboard

---

## 📖 Data Dictionary

Key columns in `Shopify Sales.xlsx`:

| Column | Description |
|--------|-------------|
| **Order Number** | Unique sequential ID assigned to each customer order |
| **Customer ID** | System-generated unique identifier per customer |
| **Gateway** | Payment processing service used (Shopify Payments, PayPal, Amazon, Gift Card, Manual) |
| **Product Type** | Category of the purchased item (Running Shoes, Tennis Shoes, Cycling Shoes, etc.) |
| **Net Sales** | Total revenue before tax |
| **Total Tax** | Tax amount applied to the order |
| **Total Price USD** | Final amount paid including tax, normalized to USD |
| **Province / City** | Customer location from billing address |
| **Quantity** | Number of units purchased in the order |
| **Invoice Date** | Date the transaction was completed |

---

## 💡 Business Value

This dashboard enables e-commerce managers, sales analysts, and marketing teams to:

- 📌 Track total revenue, order volume, and average order value in real time
- 📌 Identify high-value repeat customers vs one-time buyers to improve retention strategy
- 📌 Pinpoint top-performing cities and provinces for targeted regional campaigns
- 📌 Understand which payment gateways customers prefer for checkout optimization
- 📌 Determine which product types drive the most revenue to guide inventory decisions
- 📌 Analyze peak sales hours and days for smarter scheduling of marketing pushes

---

## 📬 Connect with Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Het%20Ladani-blue?logo=linkedin)](https://linkedin.com/in/het-ladani-5001bb29a/)
[![GitHub](https://img.shields.io/badge/GitHub-ladanihet2410-black?logo=github)](https://github.com/ladanihet2410)
