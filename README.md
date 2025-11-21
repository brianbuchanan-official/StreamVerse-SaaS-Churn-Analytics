
# 📊 **StreamVerse — SaaS Customer Churn & Revenue Analytics Dashboard**

**Excel + Power BI | End-to-End Data Analytics Project**

🔗 **Portfolio:** [https://brianbuchanan-official.github.io/](https://brianbuchanan-official.github.io/)
🔗 **LinkedIn:** [https://www.linkedin.com/in/brian-buchanan-616727224/](https://www.linkedin.com/in/brian-buchanan-616727224/)

---

## 🛠️ **Tech Stack & Tools**

![Power BI](https://img.shields.io/badge/Power%20BI-FAE500?style=for-the-badge\&logo=Power%20BI\&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge\&logo=Microsoft%20Excel\&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-0E76A8?style=for-the-badge\&logo=Microsoft%20PowerBI\&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Data%20Analytics-4B8BBE?style=for-the-badge)
![SaaS Analytics](https://img.shields.io/badge/SaaS%20Analytics-800000?style=for-the-badge)

---

## 🖼️ **Dashboard Preview**

![Dashboard Preview](assets/StreamVerse_Dashboard.png)

---

## 📌 **Overview**

StreamVerse is a fictional SaaS streaming service created to simulate real-world subscription analytics.
This project tracks **churn rates**, **revenue trends**, and **customer retention** over a 12-month period using Excel + Power BI.

The goal is to understand:

* Why customers churn
* How churn affects revenue
* Which customer segments have the highest lifetime value
* How subscription behavior evolves over time

This dashboard follows the same structure used by BI teams at streaming companies, SaaS products, and finance/actuarial analytics teams.

---

## ⭐ **Key Dashboard Features**

* 📉 **Churn Rate by Month** (Month 1 spike → stabilization)
* 👥 **Active Customers vs Cancels** (dual-axis trend)
* 💵 **Monthly Recurring Revenue (MRR)**
* 🌍 **Segmentation Filters** (Region, Plan Type, Has Kids)
* 📊 **LTV & ARPU** calculated dynamically
* 🔍 Interactive, filter-driven data exploration

---

## 📂 **Dataset Description**

The Excel dataset simulates **50,000+ subscription customers**, each tracked across a 12-month lifecycle.

### **Key fields include:**

| Column        | Description                            |
| ------------- | -------------------------------------- |
| Customer_ID   | Unique customer identifier             |
| Month_Index   | Month of subscription lifecycle (1–12) |
| Plan_Type     | Basic / Standard / Premium             |
| Region        | NA / EU / APAC / LATAM                 |
| Monthly_Price | Plan cost                              |
| Churn_Flag    | 1 if customer churns that month        |
| Is_Active     | 1 if subscribed that month             |
| Has_Kids      | Yes/No segmentation field              |
| MRR           | Monthly Recurring Revenue              |

The dataset reflects realistic SaaS behavior (high early churn → stable retention).

---

## 🔧 **How This Project Was Built**

### **1. Data Generation (Excel)**

* Created synthetic user profiles
* Assigned plans, regions, and add-ons
* Simulated churn behavior using probability decay
* Calculated revenue, active status, and churn flags

### **2. Data Modeling (Power BI)**

* Loaded Excel dataset into Power BI
* Established a clean star-schema model
* Created dimension tables (Plan, Region, Add-Ons)

### **3. DAX Measures**

* Computed Active Customers, Cancels, Churn %, MRR, ARPU, LTV
* Validated measure accuracy against data logic

### **4. Dashboard Design**

* Built clean visuals with consistent formatting
* Added slicers for Region, Plan Type, and Kids addon
* Designed professional KPI cards and charts

---

## 📊 **KPI Definitions (DAX)**

### **Churn Rate (%)**

```DAX
Churn_Pct =
DIVIDE([Cancels], [Active_Customers])
```

### **Active Customers**

```DAX
Active_Customers =
SUM(Fact_Monthly[Is_Active])
```

### **Cancelations**

```DAX
Cancels =
SUM(Fact_Monthly[Churn_Flag])
```

### **MRR**

```DAX
MRR_Monthly =
SUM(Fact_Monthly[MRR])
```

### **ARPU**

```DAX
ARPU =
DIVIDE([MRR], [Active_Customers])
```

### **Lifetime Value**

```DAX
LTV =
DIVIDE([ARPU], [Churn_Pct])
```

---

## 🔍 **Dashboard Insights**

* ⚠️ **Churn peaks heavily in Month 1**, then drops sharply
* 📈 **MRR increases each month**, despite churn
* 🏆 **Premium subscribers churn far less** than Basic customers
* 🌍 **EU & NA regions show the best retention**
* 👪 **Customers with Kids add-on have longer subscription lifetimes**

---

## 📦 **Download the Files**

* 📊 **Power BI Dashboard (.pbix)**
* 📈 **Excel Dataset (Simulated)**

Both included in this repository:

```
StreamVerse_SaaS_ChurnDashboard.pbix
StreamVerse_ChurnProject.xlsx
assets/StreamVerse_Dashboard.png
```

---

## 🚀 **Future Enhancements**

* Predictive churn model (Logistic Regression / XGBoost)
* Cohort retention dashboard
* CAC & NRR calculations
* SQL + cloud data warehouse version (Snowflake/BigQuery)

---

## 🎯 **What This Project Demonstrates**

This project shows:

* End-to-end analytics workflow
* SaaS business metric understanding
* Strong Power BI and DAX skills
* Ability to model customer behavior
* Dashboard design + storytelling
* Skills directly applicable to **data analyst**, **BI analyst**, **actuarial**, and **financial analytics** roles

---

## 👤 **Contact**

Connect with me for analytics, BI, finance, or actuarial roles:

🔗 **LinkedIn:** [https://www.linkedin.com/in/brian-buchanan-616727224/](https://www.linkedin.com/in/brian-buchanan-616727224/)
🌐 **Portfolio:** [https://brianbuchanan-official.github.io/](https://brianbuchanan-official.github.io/)

---

