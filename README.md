# 📊 Customer Segmentation & Retention Analytics in Power BI

> **MBA Portfolio Project | Customer Analytics | Segmentation | Retention Dashboard**

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Domain](https://img.shields.io/badge/Domain-Customer%20Analytics-blue)

---

## ⬇️ Download Project Files

| File | Description | Link |
|------|-------------|------|
| 📊 Power BI Dashboard | Full .pbix file with data model, DAX measures & visuals | [Download PBIX](https://github.com/atishey4/customer-analytics-powerbi-dashboard/raw/main/Customer_Analytics_Dashboard.pbix) |

---

## 📸 Screenshots

![Dashboard](screenshots/Screenshot%202026-04-16%20204249.png)

---

## 📌 Overview
This project focuses on analyzing customer behavior, segmenting customers based on value and engagement, and evaluating retention patterns using Power BI.

The dashboard is designed to help businesses identify high-value customers, detect churn risks, and improve retention strategies through data-driven insights.

---

## 🎯 Objective
To build an end-to-end Power BI dashboard that:
- Segments customers based on purchasing behavior
- Tracks retention and churn trends
- Helps businesses improve customer lifetime value (CLV)
- Supports data-driven decision-making in marketing and CRM

---

## 🧠 Business Context
Customer retention is critical for sustainable growth:
- Retaining customers is **5x cheaper** than acquiring new ones
- A small percentage of customers often contributes to the majority of revenue
- Businesses use analytics dashboards to optimize targeting, loyalty programs, and engagement strategies

---

## 🛠️ Tools & Technologies
- Power BI (Data Modeling & Visualization)
- Power Query (Data Cleaning & Transformation)
- DAX (Measures & Calculations)
- CSV Datasets

---

## 📂 Dataset Description

### 1. Customers.csv
- Customer ID, Name, Gender, Age, Region, Join Date

### 2. Transactions.csv
- Transaction ID, Customer ID, Date, Product, Quantity, Price

### 3. SupportTickets.csv (Optional)
- Ticket ID, Customer ID, Issue Type, Resolution Time

---

## ⚙️ Data Preparation (Power Query)
Key steps performed:
- Removed null values and duplicates
- Standardized data types (dates, numeric fields)
- Created calculated column:
  - **Sales Amount = Quantity × Price**
- Formatted date columns for time analysis
- Ensured clean and structured datasets while keeping raw data unchanged

---

## 🧩 Data Modeling
- Built a **Star Schema**:
  - Fact Table → Transactions
  - Dimension Table → Customers
- Relationships:
  - `Transactions[Customer ID] → Customers[Customer ID]`
- Created a **Date Table** for time intelligence:
  - Enabled trend and retention analysis

---

## 📊 Key DAX Measures

- **Total Revenue** = SUM(Sales Amount)
- **Total Customers** = DISTINCTCOUNT(Customer ID)
- **Average Order Value (AOV)** = Revenue / Orders
- **Customer Lifetime Value (CLV)**
- **Retention Rate %**
- **Churn Rate %**
- **Repeat Customers**
- **Active Customers**
- **Segment-wise Revenue**

---

## 👥 Customer Segmentation Logic

Customers were categorized into:
- **High Value** → CLV > threshold
- **Medium Value**
- **Low Value**

Additional classifications:
- **Customer Type** → New vs Returning
- **Retention Status** → Retained / At Risk / Churned

---

## 📈 Dashboard Features

### 🔹 KPI Cards
- Total Customers
- Total Revenue
- Retention Rate
- Churn Rate
- Average Order Value (AOV)

### 🔹 Visualizations
- Bar Chart → Customer Segment vs Revenue
- Column Chart → Revenue Distribution
- Donut Chart → Retention Status
- Line Chart → Retention Trend Over Time
- Cohort Heatmap → Retention Analysis
- Matrix Table → Segment vs Revenue vs Retention

### 🔹 Filters (Slicers)
- Region
- Gender
- Customer Segment
- Channel
- Date

---

## 🎨 Dashboard Design
- Corporate color theme (Blue, Green, subtle Red for churn risk)
- Clean and structured layout:
  - Top → KPI Cards
  - Middle → Charts
  - Bottom → Matrix & insights
  - Side → Filters
- Consistent fonts and spacing for professional presentation

---

## 🔍 Key Insights

- High-value customers contribute a significant portion of revenue
- A segment of customers shows high churn risk due to low engagement
- Certain regions and channels outperform others in retention
- Retention trends highlight opportunities for targeted campaigns

---

## 💼 Business Impact
This dashboard helps:
- Marketing teams → run targeted campaigns
- CRM teams → improve engagement strategies
- Management → monitor retention and revenue trends
- Businesses → increase profitability through better customer understanding

---

## 📁 Folder Structure

```
customer-analytics-powerbi-dashboard/
│
├── Customer_Analytics_Dashboard.pbix   # Main Power BI file
│
├── raw data/
│   ├── Customers.csv
│   ├── Transactions.csv
│   └── SupportTickets.csv
│
├── screenshots/
│   └── Screenshot 2026-04-16 204249.png
│
└── README.md
```

---

## 👤 Author

**Atishey Jain**  
MBA Student | IMI Delhi  
🔗 [GitHub](https://github.com/atishey4) | [LinkedIn](https://www.linkedin.com/in/atishey-jain-66430715b/)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
