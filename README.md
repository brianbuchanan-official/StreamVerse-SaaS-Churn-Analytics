
```md
# 📊 StreamVerse — SaaS Customer Churn & Revenue Analytics Dashboard

![Dashboard Preview](assets/StreamVerse_Dashboard.png)

A complete end-to-end SaaS analytics project covering churn modeling, revenue forecasting, customer behavior analysis, and interactive dashboard development using **Power BI, Excel, DAX, and SQL-style logic**.

This project is designed to mirror the analytical style used by real SaaS companies and is optimized for recruiters, hiring managers, and data teams reviewing my portfolio.

---

## 🔥 Key Features

✔ **Full SaaS KPI Suite:** Churn Rate, MRR, ARR, LTV, ARPU  
✔ **Month-by-Month cohort behavior**  
✔ **Dynamic Power BI dashboard with slicers**  
✔ **Excel-based data model & DAX formulas**  
✔ **Churn curve visualization**  
✔ **Active customers vs cancellations trend**  
✔ **MRR growth and cohort revenue trajectory**  
✔ **Complete business explanations for each metric**  
✔ **Real-world SaaS story framing for recruiters**

---

## 🚀 Project Purpose

The goal of StreamVerse is to simulate how a subscription-based business tracks and understands customer retention and revenue behavior.  
This project demonstrates:

- Strong analytical thinking  
- Ability to build end-to-end BI solutions  
- Business-oriented storytelling  
- Technical proficiency in DAX, Excel modeling, and visualization  
- Understanding of SaaS metrics used in finance, product, and data teams  

---

# 🧩 1. Dataset Overview

**Rows:** 4,536  
**Columns include:**  
- Customer_ID  
- Region (APAC, EU, LATAM, NA)  
- Plan_Type (Basic, Standard, Premium)  
- Has_Kids (Yes/No)  
- Month_Index (1–12)  
- Monthly_Price  
- Churn_Flag  
- Active_Customers  
- Cancellations  
- MRR, LTV, ARPU  
- Randomized modifiers for realism

This dataset was generated using business-driven assumptions to mimic a real SaaS platform's behavior.

---

# 📈 2. KPIs and Business Meaning

### **🟦 Active Customers**
Total customers still subscribed in the current period.

### **🟥 Cancellations**
Customers who churned / stopped paying.

### **🟩 MRR — Monthly Recurring Revenue**
Revenue generated from active customers in a given month.

### **🟨 Churn Rate (%)**
Percentage of customers who cancel.

Formula:
```

Churn Rate = Cancels / Active Customers

```

### **🟧 LTV — Lifetime Value**
Expected revenue per customer over their tenure.

Formula:
```

LTV = ARPU / Churn Rate

````

### **🟪 ARPU — Average Revenue Per User**
Total revenue / total users.

---

# 🛠️ 3. Tech Stack

### **BI & Visualization**
- Power BI  
- DAX  
- Power Query  

### **Data Modeling**
- Excel  
- Pivot modeling  
- Subscription simulation logic  

### **Project Management**
- GitHub  
- Documentation  
- Version control  

---

# 🧠 4. How the Project Was Built (Step-by-Step)

### **1. Simulated SaaS Dataset (Excel)**
- Built price tiers  
- Applied churn multipliers per region, plan type, add-ons  
- Generated Month_Index progression  
- Added realistic churn and retention patterns  
- Created revenue formulas and KPIs

### **2. Imported Into Power BI**
- Cleaned data  
- Created relationships  
- Converted flags to measures  

### **3. Built DAX Measures**
Examples:

```DAX
Churn_Pct = DIVIDE([Cancels], [Active_Customers])
````

```DAX
MRR_Monthly = SUM(Fact_Monthly[Revenue])
```

```DAX
LTV = DIVIDE([ARPU], [Churn_Pct])
```

### **4. Designed Power BI Dashboard**

* Churn trend line
* Active customers vs cancels combined chart
* MRR growth area chart
* Slicers for demographic segmentation

### **5. Exported Dashboard Image**

Used as project preview and GitHub social thumbnail.

---

# 🎨 5. Visuals Included

This README includes:

✔ Dashboard Preview
✔ KPI Cards
✔ Churn Curve
✔ MRR Growth Chart
✔ Active Customers vs Cancels

Screenshots stored in:

```
/assets/StreamVerse_Dashboard.png
```

---

# 📌 6. Project Insights & Summary

### 🔹 **Churn naturally declines over time**

Month 1 shows the highest churn (60%+), then stabilizes below 10%.

### 🔹 **Active customer base steadily grows**

Even with churn, new cohorts create growth.

### 🔹 **MRR shows strong upward momentum**

Revenue grows as churn stabilizes and customer base expands.

### 🔹 **Premium plans show lower churn + higher revenue**

Simulating typical SaaS behavior.

---

# 💼 7. Resume-Ready Impact Statement

**"Built a complete SaaS churn and revenue analytics system using Excel, Power BI, and DAX. Developed cohort-based churn trends, MRR forecasting logic, LTV modeling, and interactive dashboards with demographic segmentation. Demonstrates strong skills in BI reporting, metric design, and data-driven storytelling—mirroring analytics workflows used in real SaaS companies."**

You can paste this into your resume under Projects.

---

# 🌐 8. Links

### 🔗 **Live Portfolio Website**

[https://brianbuchanan-official.github.io/](https://brianbuchanan-official.github.io/)

### 🔗 **LinkedIn Profile**

[https://www.linkedin.com/in/brian-buchanan-616727224/](https://www.linkedin.com/in/brian-buchanan-616727224/)

---

# 🧩 9. Files in This Repository

| File                                     | Description             |
| ---------------------------------------- | ----------------------- |
| **StreamVerse_ChurnProject.xlsx**        | Full Excel data model   |
| **StreamVerse_SaaS_ChurnDashboard.pbix** | Power BI dashboard      |
| **StreamVerse_Dashboard.png**            | Dashboard preview image |
| **README.md**                            | Project documentation   |

---

# 🔥 10. Recruiter-Friendly Summary (TL;DR)

This project shows:

✔ Strong BI & analytics skills
✔ SaaS metric expertise
✔ Dashboard design + storytelling
✔ Data modeling & DAX proficiency
✔ End-to-end problem-solving
✔ Real-world business thinking

Exactly what analytics, finance, and tech hiring managers are looking for.

---

# ⭐ 11. Future Enhancements

* Add SQL database migration
* Build Python simulator for more realistic cohort modeling
* Add Net Revenue Retention (NRR) + Gross Revenue Retention (GRR)
* Export dashboard to interactive web embed

---

# 📬 Contact

If you'd like to discuss this project or the analytics behind it:

* **LinkedIn:** [https://www.linkedin.com/in/brian-buchanan-616727224/](https://www.linkedin.com/in/brian-buchanan-616727224/)
* **Portfolio Website:** [https://brianbuchanan-official.github.io/](https://brianbuchanan-official.github.io/)

(No email displayed publicly for privacy.)

---
