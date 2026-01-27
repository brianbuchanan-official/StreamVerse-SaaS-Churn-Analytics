# StreamVerse — SaaS Customer Churn & Revenue Analytics

## Executive Summary

Subscription-based businesses depend on retention and recurring revenue stability to sustain growth. This project evaluates customer churn behavior, revenue dynamics, and cohort performance using a simulated SaaS dataset, translating raw subscription activity into decision-ready KPIs and executive dashboards. The analysis is designed to support retention strategy, pricing evaluation, and revenue forecasting decisions.

**Scope (Locked):**
- Monthly churn analysis (12-month horizon)
- KPI focus: Churn Rate, MRR, ARR, ARPU, LTV
- Cohort-based customer behavior
- Region and plan segmentation
- Tools: Excel (data model) + Power BI (executive dashboard)
- Simulated dataset reflecting real SaaS operating behavior

---

## Deliverables

- **Excel Model:**  
  `StreamVerse_ChurnProject.xlsx`

- **Power BI Dashboard:**  
  `StreamVerse_SaaS_ChurnDashboard.pbix`

- **Executive Dashboard Preview:**  
  `assets/StreamVerse_Dashboard.png`

---

## Executive KPI Overview (Power BI Dashboard)

![StreamVerse Executive Dashboard](assets/StreamVerse_Dashboard.png)

---

## Business Problem

Recurring revenue businesses must manage churn proactively to protect growth and long-term customer value. Revenue expansion alone does not guarantee sustainability if customer attrition erodes the active base or compresses lifetime value.

**Executive Question:**  
**How do churn patterns, customer cohorts, and pricing tiers affect revenue stability and long-term customer value?**

---

## Key Performance Indicators (KPIs)

- Active Customers  
- Cancellations  
- Churn Rate  
- Monthly Recurring Revenue (MRR)  
- Annual Recurring Revenue (ARR)  
- Average Revenue per User (ARPU)  
- Lifetime Value (LTV)

---

## Data & Methodology

The dataset consists of **4,536 simulated customer-month observations** across a 12-month lifecycle. Customers are segmented by region, subscription tier, and product attributes. Churn behavior is introduced through structured assumptions reflecting early-life churn, cohort stabilization, and tier-based retention differences.

Revenue metrics are calculated at the monthly level and aggregated using Power BI measures. Churn rate is computed as cancellations divided by active customers. Lifetime value is estimated using a steady-state churn assumption.

---

## Key Findings

- Churn is highest during early subscription periods and stabilizes over time.
- Premium-tier customers exhibit lower churn and higher lifetime value.
- Revenue growth is driven more by retention stability than raw customer acquisition.
- Cohort analysis reveals materially different revenue trajectories across customer segments.

---

## Recommendations

- Prioritize early-life retention initiatives to reduce first-period churn.
- Focus pricing and feature investment on higher-retention tiers.
- Monitor cohort-level churn rather than relying solely on aggregate metrics.
- Use churn-adjusted LTV as a primary input for marketing and acquisition strategy.

---

## Next Steps (Write-Up Only)

- Migrate the dataset to a relational SQL database for scalable analysis.
- Introduce Net Revenue Retention (NRR) and Gross Revenue Retention (GRR).
- Extend cohort modeling using Python for probabilistic churn simulation.
- Embed dashboard views into a web-based analytics interface.

---

## Files Included

| File                                 | Description              |
|-------------------------------------|--------------------------|
| StreamVerse_ChurnProject.xlsx        | Excel data model         |
| StreamVerse_SaaS_ChurnDashboard.pbix | Power BI dashboard       |
| assets/StreamVerse_Dashboard.png    | Executive dashboard view |
| README.md                            | Project documentation   |
