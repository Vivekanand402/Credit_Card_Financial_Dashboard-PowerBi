# Credit_Card_Financial_Dashboard-PowerBi
# 💳 Credit Card Financial Dashboard

## 📊 Project Overview

The **Credit Card Financial Dashboard** is an interactive **Power BI data analytics project** designed to analyze credit card transactions and customer information.

The dashboard provides insights into key financial and customer performance metrics, helping stakeholders monitor trends, identify business opportunities, and support data-driven decision-making.

---

## 🎯 Project Objective

The main objective of this project is to develop a comprehensive **Credit Card Weekly Dashboard** that provides insights into key performance metrics and trends.

The dashboard enables stakeholders to effectively monitor and analyze credit card operations through interactive visualizations and business KPIs.

---

## 🛠️ Tools & Technologies

* **Power BI** – Dashboard development & data visualization
* **SQL** – Data storage, querying & data extraction
* **DAX** – Calculated columns, measures & KPI calculations
* **CSV** – Source data
* **Data Analysis** – Business insights & performance analysis

---

## 🔄 Project Workflow

```text
CSV Dataset
     ↓
SQL Database
     ↓
Data Cleaning & Processing
     ↓
DAX Calculations
     ↓
Power BI Dashboard
     ↓
Business Insights
     ↓
Decision Making
```

---

## 🗄️ Data Preparation

The project data was imported into a SQL database before connecting it with Power BI.

### Steps:

1. Prepared CSV files
2. Created tables in SQL
3. Imported CSV data into SQL
4. Queried and analyzed the data
5. Connected SQL data with Power BI
6. Performed data processing and transformation

---

## 📐 DAX Calculations

Several DAX calculations were created to analyze customer and financial data.

### Age Group Classification

```DAX
AgeGroup =
SWITCH(
    TRUE(),
    'public cust_detail'[customer_age] < 30, "20-30",
    'public cust_detail'[customer_age] >= 30 &&
    'public cust_detail'[customer_age] < 40, "30-40",
    'public cust_detail'[customer_age] >= 40 &&
    'public cust_detail'[customer_age] < 50, "40-50",
    'public cust_detail'[customer_age] >= 50 &&
    'public cust_detail'[customer_age] < 60, "50-60",
    'public cust_detail'[customer_age] >= 60, "60+",
    "Unknown"
)
```

### Income Group Classification

```DAX
IncomeGroup =
SWITCH(
    TRUE(),
    'public cust_detail'[income] < 35000, "Low",
    'public cust_detail'[income] >= 35000 &&
    'public cust_detail'[income] < 70000, "Medium",
    'public cust_detail'[income] >= 70000, "High",
    "Unknown"
)
```

### Revenue Calculation

```DAX
Revenue =
'public cc_detail'[annual_fees]
+ 'public cc_detail'[total_trans_amt]
+ 'public cc_detail'[interest_earned]
```

### Week-over-Week Revenue Analysis

The dashboard also calculates current-week and previous-week revenue to analyze **WoW (Week-over-Week) performance**.

---

## 📊 Key KPIs

The dashboard focuses on important financial and customer metrics such as:

* 💰 Total Revenue
* 💳 Total Transaction Amount
* 🔢 Transaction Count
* 👥 Customer Count
* 💵 Interest Earned
* 📈 Week-over-Week Revenue
* ⚡ Activation Rate
* ⚠️ Delinquent Rate
* 💳 Credit Card Performance
* 👤 Customer Demographics

---

## 🔍 Key Business Insights

Based on the dashboard analysis:

* Revenue increased by **28.8% Week-over-Week**.
* Overall Year-to-Date revenue reached approximately **57M**.
* Total interest earned was approximately **8M**.
* Total transaction amount was approximately **46M**.
* Male customers contributed approximately **31M** in revenue, compared with **26M** from female customers.
* **Blue and Silver credit cards** contributed approximately **93%** of overall transactions.
* **Texas, New York and California** contributed approximately **68%** of the overall performance.
* Overall activation rate was approximately **57.5%**.
* Overall delinquent rate was approximately **6.06%**.

---

## 📈 Dashboard Features

The Power BI dashboard provides:

* Interactive KPI cards
* Weekly performance analysis
* Customer demographic analysis
* Revenue analysis
* Transaction analysis
* Credit card category analysis
* Geographic performance analysis
* Customer segmentation
* Week-over-Week comparison

---

## 💼 Business Value

This dashboard can help businesses:

* Monitor financial performance
* Track customer transaction behavior
* Identify high-performing customer segments
* Analyze revenue trends
* Monitor activation and delinquency rates
* Identify regional performance
* Support data-driven business decisions

---

## 📂 Project Structure

```text
Credit-Card-Financial-Dashboard/
│
├── Dataset/
│   └── credit_card_data.csv
│
├── SQL/
│   └── SQL_Queries.sql
│
├── PowerBI/
│   └── Credit_Card_Dashboard.pbix
│
├── Screenshots/
│   └── dashboard.png
│
└── README.md
```

---

## 🚀 How to Use

1. Download or clone this repository.
2. Import the dataset into your SQL database.
3. Execute the required SQL queries.
4. Open the Power BI `.pbix` file.
5. Update the database connection if required.
6. Refresh the dataset.
7. Explore the interactive dashboard.

---

## 🎓 Skills Demonstrated

This project demonstrates practical knowledge of:

**SQL | Power BI | DAX | Data Cleaning | Data Transformation | Data Visualization | KPI Development | Business Intelligence | Business Analysis | Dashboard Development**

---

## 👨‍💻 Author

**Vivekanand Dubey**

Aspiring **Data Analyst | Business Intelligence Enthusiast**

### Skills

* SQL
* Power BI
* DAX
* Excel
* Python
* Data Analytics
* Data Visualization
* Business Intelligence

