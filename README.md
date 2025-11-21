# **StreamVerse — Customer Churn & Revenue Dashboard**

A full SaaS analytics dashboard built using **Power BI + Excel**, designed to analyze customer churn, revenue performance, and retention behavior across a 12-month period.

🔗 **Portfolio Website:** [https://brianbuchanan-official.github.io/](https://brianbuchanan-official.github.io/)
🔗 **LinkedIn:** [https://www.linkedin.com/in/brian-buchanan-616727224/](https://www.linkedin.com/in/brian-buchanan-616727224/)

---

## 🖼️ **Dashboard Preview**

![Dashboard Preview](assets/StreamVerse_Dashboard.png)

---

## 📌 **Overview**

StreamVerse is a simulated SaaS subscription analytics project created to demonstrate the ability to analyze customer behavior, identify churn risks, and evaluate key subscription KPIs.
This dashboard helps stakeholders understand:

* Why customers churn
* How churn impacts revenue
* How different plans & customer segments behave
* How customer value evolves over time

The project is fully interactive, filter-driven, and appropriate for real-world SaaS product teams.

---

## ⭐ **Key Features**

* 📉 **Churn Rate Tracking** across all 12 months
* 👥 **Active Customers & Cancelations** visualized together
* 💵 **Monthly Recurring Revenue (MRR)** growth chart
* 🎯 **Customer LTV (Lifetime Value)** calculation
* 💳 **ARPU (Average Revenue Per User)**
* 🌍 **Segmentation by Region, Plan Type, and Family Indicators**
* 📊 Fully interactive Power BI dashboard

---

## 📁 **Dataset Description**

The dataset simulates **50,000 SaaS subscribers** over a one-year period.

### **Key fields include:**

* `Customer_ID` – unique user
* `Month_Index` – month of the customer lifecycle (1–12)
* `MRR` – monthly recurring revenue
* `Monthly_Price` – price based on selected plan
* `Plan_Type` – Basic / Standard / Premium
* `Region` – NA / EU / APAC / LATAM
* `Churn_Flag` – 1 if customer cancels that month
* `Has_Kids`, `Has_Sports` – segmentation attributes

The Excel file powering all visuals is included in the repo.

---

## 🔢 **Core DAX Calculations**

### **Churn Rate (%)**

```DAX
Churn_Pct =
VAR MonthlyActive = CALCULATE([Active_Customers])
VAR MonthlyCancels = CALCULATE([Cancels])
RETURN DIVIDE(MonthlyCancels, MonthlyActive)
```

### **Active Customers**

```DAX
Active_Customers = SUM(Fact_Monthly[Is_Active])
```

### **Monthly Cancels**

```DAX
Cancels = SUM(Fact_Monthly[Churn_Flag])
```

### **Monthly Recurring Revenue (MRR)**

```DAX
MRR_Monthly = SUM(Fact_Monthly[MRR])
```

### **LTV**

```DAX
LTV = DIVIDE([ARPU], [Churn_Pct])
```

### **ARPU**

```DAX
ARPU = AVERAGE(Fact_Monthly[Monthly_Price])
```

---

## 📊 **Dashboard Insights**

* 🔻 **Churn rate drops from ~68% to ~4%** after customers stay past Month 2
* 📈 **MRR grows steadily** each month as more customers join than churn
* 🏆 **Premium users show higher retention** and contribute more revenue
* 🌍 **EU and NA have the strongest retention stability**
* 👪 Customers with kids have slightly lower churn on average

---

## 🕹️ **How to Use This Dashboard**

1. Download the `.pbix` or Excel dataset from this repository
2. Open in Power BI Desktop
3. Use slicers on the right side to filter by:

   * Region
   * Plan_Type
   * Has_Kids
4. Hover and interact with visuals to explore churn trends and revenue patterns

---

## 📦 **Repository Contents**

```
├── assets/
│   └── StreamVerse_Dashboard.png
├── StreamVerse_ChurnProject.xlsx
├── StreamVerse_SaaS_ChurnDashboard.pbix
└── README.md
```

---

## 📬 **Contact**

I’m open to opportunities in **data analytics, business intelligence, actuarial analysis, and financial analytics**.

🔗 **LinkedIn:** [https://www.linkedin.com/in/brian-buchanan-616727224/](https://www.linkedin.com/in/brian-buchanan-616727224/)
🌐 **Portfolio:** [https://brianbuchanan-official.github.io/](https://brianbuchanan-official.github.io/)

*No email included for privacy — connect with me on LinkedIn.*

