Churn Analysis & Customer Intelligence

1. Project Overview

An end-to-end Customer Churn Analysis project for an OTT subscription platform. The objective is to identify high-risk customers, understand the key drivers of churn, quantify revenue impact, and recommend actionable retention strategies.

This project combines SQL and Python to extract, clean, transform, analyze, and visualize customer data from multiple relational tables.

---

2. Business Challenge

In the highly competitive OTT industry, customer retention is critical for sustainable revenue growth.

The objective of this project is to answer three key business questions:

- Who is churning or at high risk of churn?
- Why are customers leaving?
- When does a customer enter the danger zone?

The analysis focuses on customer demographics, subscription plans, contract types, customer tenure, churn scores, and support interactions.

---

3. Tech Stack & Libraries

Programming & Database

- Python
- SQL
- SQLite

Python Libraries

- Pandas – Data manipulation and analysis
- NumPy – Numerical calculations and feature engineering
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- sqlite3 – Connecting Python with SQLite database

Analytics

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- KPI Analysis
- Customer Segmentation
- Behavioral Analysis
- Business Insights

---

4. Database Structure

The project uses a SQLite database named customer_churn.db containing three relational tables.

db_customer

- customerid
- name
- country
- state
- gender
- dob
- interests
- pincode

db_subscription

- customerid
- subscription_start_date
- subscription_type
- renewal_date
- plan_type
- contract_type
- cancellation_date
- cancellation_reason
- monthly_charges
- cltv
- churn_score

db_support

- customerid
- complaint_date
- escalations
- csat_score
- comment

---

5. Project Roadmap

Step 1 – Connect SQL Database to Python

- Connect SQLite database with Python
- Use "sqlite3" and "pandas"
- Extract data using SQL queries

Step 2 – Data Import

- Import multiple relational tables
- Join customer, subscription, and support data
- Create an analysis-ready dataset

Step 3 – Data Cleaning

- Check data types
- Rename columns
- Select required columns
- Perform quality checks
- Handle missing/null values
- Remove inconsistencies

Step 4 – Feature Engineering

- Calculate customer tenure
- Calculate churn indicators
- Create calculated columns
- Transform data
- Apply business filters

Step 5 – Data Analysis

- Calculate KPIs
- Group-by analysis
- Aggregations
- Pivot tables
- Customer segmentation

Step 6 – Exploratory Data Analysis

Analyze churn based on:

- Plan type
- Contract type
- State
- Customer tenure
- Monthly charges
- Churn score
- Support escalations

Step 7 – Data Visualization

Create visualizations using:

- Matplotlib
- Seaborn

Step 8 – Business Insights

Translate analytical findings into:

- Key insights
- Revenue impact
- Customer risk areas
- Retention strategies
- Recommended next steps

---

6. Business Definition of Churn

Business Type| Churn Definition
SaaS| Subscription cancelled
E-commerce| No purchase in 90 days
AdTech| No service/app usage for 90–120 days
Streaming| Membership inactive
Telecom| Account terminated
Banking| No transactions for X months

For this OTT project:

Churn = Customer membership/subscription becoming inactive or being cancelled.

---

7. Key Performance Indicators (KPIs)

KPI| Formula
Churn Rate| Churned Customers / Total Customers
Retention Rate| 1 - Churn Rate
Churn by Plan| Churn Rate GROUP BY Plan Type
Churn by State| Churn Rate GROUP BY Country, State
ARPU| Total Monthly Charges / Active Customers
Average Customer Tenure| Average subscription duration
Revenue at Risk| Monthly Charges where Churn Score > 70
Escalation Rate| Escalations / Complaints × 100
Avg. Complaints per Customer| Complaints / Distinct Customers
Escalation → Churn| Churn Rate for customers with escalations vs. without

---

8. Key Insights

- Overall Churn Rate: 28.6%
- Retention Rate: 71.4%
- Monthly Contract Churn: 55.6%
- Annual Contract Churn: 8.3%
- Monthly-contract customers show approximately 6.7× higher churn than annual-contract customers.
- Most churn is concentrated in the Basic subscription plan.
- September 2024 recorded the highest churn.
- Karnataka was the most affected state.
- Average Customer Tenure: 1,451 days
- ARPU: ₹18.8
- Total Revenue: 395
- Revenue Loss due to Churn: approximately 74
- Revenue Loss: approximately 18%
- CLTV Lost: 2,047

«Note: Metrics are based on the project dataset and may change if the underlying database is updated.»

---

9. Business Recommendations

1. Investigate Karnataka Churn

Analyze whether the increase was related to:

- Pricing changes
- Technical issues
- Customer complaints
- Content availability
- Competitor activity

2. Reduce Monthly-Plan Churn

Investigate why monthly subscribers churn at a significantly higher rate than annual subscribers.

Consider:

- Annual-plan migration offers
- Loyalty discounts
- Longer-term subscription incentives

3. Target High-Risk Customers

Prioritize customers with:

- High churn scores
- Medium churn scores
- High CLTV
- Multiple complaints
- Support escalations

Use targeted:

- Emails
- SMS
- Calls
- Personalized offers

4. Monitor Competitor Switching

Investigate customers who cancel because of competitor offerings and compare:

- Pricing
- Content
- Features
- Customer experience

---

10. Portfolio Project Summary

Churn & Revenue Impact

Engineered an end-to-end churn analytics pipeline for an OTT subscription dataset by integrating customer, subscription, and support data across three relational tables and calculating 20+ business KPIs.

The analysis identified a 28.6% overall churn rate, with monthly-contract subscribers showing 55.6% churn compared with 8.3% for annual subscribers. The analysis also quantified approximately 74 in revenue loss and 2,047 in CLTV loss, enabling a targeted retention strategy focused on high-risk customers.

Risk Scoring & Segmentation

Developed a multi-dimensional customer risk analysis using subscription tenure, plan type, contract type, churn score, and support escalation signals.

Customers were segmented into risk categories to identify high-value customers requiring immediate retention intervention.

Support Intelligence

Analyzed the relationship between customer complaints, support escalations, CSAT scores, and churn to identify potential customer-experience drivers behind cancellations.

---

11. Business Impact

The analysis can help an OTT business:

- Identify customers at risk of churn
- Reduce revenue leakage
- Improve customer retention
- Prioritize high-value customers
- Understand subscription behavior
- Optimize monthly vs. annual plans
- Improve customer support strategy
- Build targeted retention campaigns

---

12. Project Structure

Churn-Analysis/
├── Churn_Analysis.ipynb
├── customer.xlsx
└── README.md

---

13. Conclusion

This project demonstrates how SQL + Python + Data Analytics can be used to convert raw customer data into actionable business decisions.

The focus is not only on calculating churn, but on understanding who is leaving, why they are leaving, when they are most likely to leave, and how the business can intervene before revenue is lost.

---

Skills Demonstrated

SQL | Python | Pandas | NumPy | SQLite | Matplotlib | Seaborn | Data Cleaning | Feature Engineering | EDA | Customer Segmentation | KPI Analysis | Business Intelligence | Data Visualization | Actionable Insights
