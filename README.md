📊 StreamVerse — SaaS Customer Churn & Revenue Analytics

Power BI + Excel | End-to-End Analytics Case Study

This project analyzes customer churn, retention, and monthly recurring revenue (MRR) for a fictional streaming service called StreamVerse.
It showcases real business KPIs, SQL-style data modeling logic (via Power BI), and a full analytics workflow from raw data → insights → dashboard.

🚀 Project Overview

StreamVerse operates as a SaaS subscription service with multiple plan types and add-ons.
This project simulates 12 months of customer behavior and evaluates:

Churn rate

Active customers

Monthly recurring revenue (MRR)

Lifetime value (LTV)

Average revenue per user (ARPU)

The goal is to understand how customer behavior evolves over time and how subscription revenue scales.

🛠️ Tools & Technologies

Power BI Desktop – dashboard, DAX measures

Excel – dataset design and logic

DAX – data modelling & KPI creation

GitHub – version control + project documentation

📈 Key KPIs

These metrics were calculated using custom DAX and aggregated across 12 months:

KPI	Description
Active Customers	Total customers currently subscribed
Cancels	Total customer cancellations
Churn Rate (%)	Cancels ÷ Active Customers
MRR	Total recurring subscription revenue
LTV	Lifetime value per customer
ARPU	Average revenue per active subscriber
📊 Dashboard Preview

(When you're ready, export the dashboard as an image and upload it… I’ll help embed it.)

📁 Project Files
File	Description
StreamVerse_ChurnProject.xlsx	Fully simulated dataset with 4,500+ customers over 12 months
StreamVerse_SaaS_ChurnDashboard.pbix	Power BI dashboard with KPIs, churn trend, cancellations, MRR trend, and segments
🔍 Analysis Highlights
1. Churn Rate Drops Over Time

Customers show high churn in Month 1 (typical onboarding churn), but retention improves dramatically by Month 6–12.

2. Active Customers Grow Steadily

Despite cancellations, growth outweighs churn due to stronger retention.

3. MRR Rises Month-Over-Month

Revenue climbs as more customers stay subscribed and upgrade plans.

4. LTV & ARPU Are Strong

High customer value suggests solid product-market fit.


-- Monthly Active Customers
Active_Customers =
CALCULATE(
    COUNTROWS(Fact_Monthly),
    Fact_Monthly[Is_Active] = 1
)

-- Monthly Cancels
Cancels =
CALCULATE(
    COUNTROWS(Fact_Monthly),
    Fact_Monthly[Churn_Flag] = 1
)

-- Churn Percentage
Churn_Pct =
DIVIDE([Cancels], [Active_Customers])

-- Monthly Revenue (MRR)
MRR_Monthly =
SUM(Fact_Monthly[Revenue])

-- Customer Lifetime Value
LTV =
DIVIDE([MRR], [Churn_Pct])

-- Average Revenue per User
ARPU =
DIVIDE([MRR], [Active_Customers])

🧠 What This Project Demonstrates

✔ Ability to build a clean, business-focused analytics dashboard
✔ Strong understanding of SaaS metrics
✔ Data modeling and DAX calculation skills
✔ Ability to turn raw data into meaningful insights
✔ Portfolio project worthy of analytics, finance, or data positions

📬 Contact

If you'd like to connect or discuss the project:

Brian Buchanan
GitHub: brianbuchanan-official
LinkedIn: (add link later)
