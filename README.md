# 🚲 Bike Store Sales Analysis Project

## 📌 Project Overview

This project analyzes the sales performance, employee productivity, and inventory management of a bicycle retail business operating across multiple stores in the United States.

The company manages nine bicycle brands including Electra, Haro, Heller, Pure Cycles, Ritchey, Strider, Sun Bicycles, Surly, and Trek, and sells products across multiple categories such as Children's Bikes, Comfort Bikes, Cruisers, Cyclocross Bikes, Electric Bikes, Mountain Bikes, and Road Bikes.

The project was developed using Microsoft Excel, Power Query, Power Pivot, Pivot Tables, Pivot Charts, and Interactive Dashboards.

---

# 🎯 Business Objectives

The objective of this project is to answer key business questions:

### Sales Analysis
- Which brands generate the highest revenue?
- Which product categories perform best?
- Which products contribute the most revenue?
- Which stores generate the highest sales?
- How do sales perform over time?

### Employee Performance Analysis
- Which employee processes the highest number of orders?
- Which employee generates the highest revenue?
- Who is the Employee of the Year?

### Inventory Analysis
- Which stores have low inventory levels?
- Which products require replenishment?
- Which categories hold the highest stock levels?
- How is inventory distributed across stores?

---

# 📂 Dataset Information

The dataset consists of nine relational tables:

| Table | Records |
|---------|---------|
| Brands | 9 |
| Categories | 7 |
| Customers | 1,445 |
| Orders | 1,615 |
| Order Items | 4,722 |
| Products | 321 |
| Staff | 10 |
| Stock | 939 |
| Stores | 3 |

---

# 🧹 Data Cleaning & Transformation

The following data preparation steps were performed:

### Customer Table
- Removed Phone Number
- Removed Street Address
- Removed Zip Code
- Standardized State Names

### Staff Table
- Combined First Name and Last Name into Full Name
- Removed Phone Number
- Removed Email Address

### Store Table
- Removed Phone Number
- Removed Email Address
- Removed Street Address
- Removed Zip Code

### General Cleaning
- Checked duplicate records
- Validated primary keys
- Corrected date data types
- Standardized state abbreviations:
  - CA → California
  - NY → New York
  - TX → Texas

---

# ⚙️ Feature Engineering

The following calculated fields were created:

### Gross Sales

Gross Sales = Quantity × List Price

Purpose:
- Measures sales before discounts

---

### Discount Amount

Discount Amount = Gross Sales × Discount

Purpose:
- Measures total discount provided

---

### Revenue

Revenue = Gross Sales − Discount Amount

Purpose:
- Primary KPI used throughout analysis

---

### Delivery Days

Delivery Days = Shipped Date − Order Date

Purpose:
- Measures delivery duration

---

### Delivery Status

Categories:
- Early Delivery
- On-Time Delivery
- Late Delivery

Purpose:
- Evaluates fulfillment performance

---

### Date Intelligence Columns

Created:
- Order Month
- Order Year
- Quarter

Purpose:
- Time-series reporting and trend analysis

---

### Inventory Metrics

Created:
- Stock Status
- Reorder Flag

Purpose:
- Inventory monitoring and replenishment planning

---

# 🔗 Data Model

Relationships were created using Power Pivot.

### Sales Model

Orders → Order Items

Order Items → Products

Products → Brands

Products → Categories

Orders → Stores

Orders → Staff

### Inventory Model

Stock → Products

Products → Brands

Products → Categories

Stock → Stores

This relational structure minimizes redundancy and improves reporting efficiency.

---

# 📊 Dashboard Overview

The project contains three interactive dashboards.

---

# Dashboard 1: Executive Sales Dashboard

<img width="812" height="486" alt="EXECUTIVE SALES DASHBOARD" src="https://github.com/user-attachments/assets/7e9f0f9c-86ab-4267-869b-b215913285c4" />


### Purpose

Provide management with a high-level overview of sales performance across products, brands, categories, stores, and time periods.




### Business Insights

- Identify top-performing brands
- Identify best-selling categories
- Analyze store performance
- Monitor sales growth trends

---

# Dashboard 2: Employee Performance Dashboard

<img width="710" height="481" alt="EMPLOYEE PERFORMANCE DASHBOARD" src="https://github.com/user-attachments/assets/5e91c5d8-857f-4484-9139-e3f5d1b9c06f" />


### Purpose

Evaluate employee productivity and contribution to business performance.



### Business Insights

- Identify top-performing employees
- Measure employee contribution to revenue
- Recognize Employee of the Year
- Support performance management decisions

---

# Dashboard 3: product performance Analysis Dashboard

<img width="701" height="485" alt="PRODUCT PERFORMANCE DASHBOARD" src="https://github.com/user-attachments/assets/e83164a1-6c0d-4163-9493-1660f883942a" />


### Purpose

Monitor inventory availability and support inventory planning decisions.




### Business Insights

- Identify low-stock products
- Improve inventory allocation
- Support replenishment planning
- Reduce stock-out risk

---

# 📈 Expected Outcomes

The analysis is expected to:

- Identify the most profitable brands and categories
- Improve store-level sales visibility
- Measure employee performance accurately
- Optimize inventory allocation
- Reduce stock shortages
- Support data-driven decision making

---

# 🛠️ Tools Used

- Microsoft Excel
- Power Query
- Power Pivot
- Pivot Tables
- Pivot Charts
- Slicers
- Data Modeling

---

# 💡 Key Skills Demonstrated

- Data Cleaning
- Data Transformation
- Data Modeling
- Exploratory Data Analysis (EDA)
- KPI Development
- Dashboard Design
- Business Analysis
- Sales Analytics
- Inventory Analytics
- Employee Performance Analytics

---

# 🚀 Project Outcome

This project delivers a complete business intelligence solution that enables management to monitor sales performance, employee productivity, and inventory levels through interactive dashboards and actionable business insights.
