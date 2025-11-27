# 📊 StreamVerse — SaaS Customer Churn & Revenue Analytics Dashboard

![Dashboard Preview](assets/StreamVerse_Dashboard.png)

A complete end-to-end SaaS analytics project covering churn modeling, revenue forecasting, customer behavior analysis, and interactive dashboard development using Power BI, Excel, DAX, and SQL-style logic.

---

## 🔥 Key Features

* Full SaaS KPI Suite: Churn Rate, MRR, ARR, LTV, ARPU
* Month-by-Month cohort behavior
* Dynamic Power BI dashboard with slicers
* Excel-based data model and DAX formulas
* Churn curve visualization
* Active customers vs cancellations trend
* MRR growth and cohort revenue trajectory
* Clear business explanations for each metric
* Recruiter-friendly SaaS storytelling

---

## 🚀 Project Purpose

StreamVerse simulates how a subscription business tracks retention and revenue.
This project demonstrates:

* Analytical thinking
* End-to-end BI workflow skills
* Data modeling and DAX proficiency
* Ability to build dashboards and interpret SaaS metrics
* Real-world business storytelling

---

## 🧩 Dataset Overview

**Rows:** 4,536
**Columns include:**

* Customer_ID
* Region (APAC, EU, LATAM, NA)
* Plan_Type (Basic, Standard, Premium)
* Has_Kids
* Month_Index (1–12)
* Monthly_Price
* Churn_Flag
* Active_Customers
* Cancellations
* MRR, LTV, ARPU

Dataset was generated with business-driven assumptions to mimic real SaaS behavior.

---

## 📈 KPIs & Business Meaning

### Active Customers

Total customers still subscribed in the period.

### Cancellations

Customers who churned.

### MRR — Monthly Recurring Revenue

Revenue from active subscribers.

### Churn Rate

```
Churn Rate = Cancels / Active Customers
```

### LTV — Lifetime Value

```
LTV = ARPU / Churn Rate
```

### ARPU — Average Revenue Per User

Total revenue divided by total customers.

---

## 🛠️ Tech Stack

**BI & Visualization**

* Power BI
* DAX
* Power Query

**Data Modeling**

* Excel
* Pivot tables
* Subscription simulation logic

**Version Control**

* GitHub
* Documentation

---

## 🧠 Build Process (Step-by-Step)

### 1. Simulated Dataset (Excel)

* Created pricing tiers
* Applied churn modifiers
* Generated Month_Index
* Added churn and retention patterns
* Calculated revenue KPIs

### 2. Imported Into Power BI

* Cleaned and shaped data
* Created relationships
* Converted columns into measures

### 3. Created DAX Measures

Examples:

```DAX
Churn_Pct = DIVIDE([Cancels], [Active_Customers])
```

```DAX
MRR_Monthly = SUM(Fact_Monthly[Revenue])
```

```DAX
LTV = DIVIDE([ARPU], [Churn_Pct])
```

### 4. Built Power BI Dashboard

* Churn trend lines
* Active vs Cancels visualization
* MRR growth
* Demographic slicers

### 5. Exported Dashboard Image

Saved for project preview.

---

## 🎨 Visuals Included

* Dashboard Preview
* KPI Cards
* Churn Curve
* MRR Growth
* Active vs Cancels

Images stored in:

```
/assets/StreamVerse_Dashboard.png
```

---

## 📌 Insights & Summary

* Churn peaks in Month 1 then normalizes
* Active customer base grows steadily
* MRR increases as churn stabilizes
* Premium users churn less and contribute more revenue

---

## 💼 Resume-Ready Statement

**Built a complete SaaS churn and revenue analytics system using Excel, Power BI, and DAX. Designed cohort-based churn modeling, MRR forecasting, LTV calculations, and interactive dashboards. Demonstrates strong BI reporting skills and real SaaS analytics expertise.**

---

## 🌐 Links

**Portfolio Website:**
[https://brianbuchanan-official.github.io/](https://brianbuchanan-official.github.io/)

**LinkedIn:**
[https://www.linkedin.com/in/brian-buchanan-616727224/](https://www.linkedin.com/in/brian-buchanan-616727224/)

---

## 📂 Files Included

| File                                 | Description        |
| ------------------------------------ | ------------------ |
| StreamVerse_ChurnProject.xlsx        | Excel model        |
| StreamVerse_SaaS_ChurnDashboard.pbix | Power BI dashboard |
| StreamVerse_Dashboard.png            | Dashboard preview  |
| README.md                            | Documentation      |

---

## ⭐ Future Enhancements

* SQL database migration
* Python-based cohort simulation
* Add NRR and GRR metrics
* Create embedded interactive web version

