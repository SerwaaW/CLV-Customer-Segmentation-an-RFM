# CLV-Customer-Segmentation-an-RFM
This repository contains the complete implementation of a project focused on Customer Segmentation and Customer Lifetime Value (CLV) analysis using SQL, data visualization tools, and cohort analysis.

**Project Overview**

This project is divided into two main tasks:

**Customer Segmentation and RFM Analysis**

Goal: Identify customer segments based on Recency, Frequency, and Monetary (RFM) scores and provide actionable insights for targeted marketing.

**Customer Lifetime Value (CLV) Analysis**

Goal: Calculate and predict CLV for customers using cohort analysis and provide insights for business growth.

**Task 1: Customer Segmentation & RFM Analysis**

**Objectives:**

- Use transactional data from 2010-12-01 to 2011-12-01 for customer segmentation.
- Calculate RFM values and scores using SQL with quartiles for segmentation.
- Create RFM-based customer segments such as Best Customers, Loyal Customers, Big Spenders, and Lost Customers.
- Present the results in a dashboard (Tableau/Power BI/Looker Studio) and provide actionable insights.

**Process:**

Data Selection & Filtering:

Extract data for the specified timeframe using SQL.

Use APPROX_QUANTILES in BigQuery to calculate RFM quartiles.

**RFM Calculation:**

Recency: Days since the customer's last transaction (calculated from 2011-12-01).

Frequency: Total number of transactions.

Monetary Value: Total spend.

**Scoring:**

Assign scores from 1 to 4 (using quartiles) for each RFM metric.

Calculate a combined RFM score.

Customer Segmentation:

Categorize customers into actionable segments based on their RFM scores.

**Visualization and Insights:**

Develop an interactive dashboard showcasing customer segmentation.

Highlight key segments for the marketing team's focus.

**Task 2: CLV Analysis**

**Objectives**:

Incorporate all user registrations (not just purchasers) into the analysis.
Perform weekly cohort analysis to predict revenue trends.
Calculate average cumulative revenue per user over a 12-week period.

**Process**

**Data Preparation:**

Use user_pseudo_id to distinguish users and identify their first visit date as their "registration date."

Calculate weekly revenue divided by weekly registrations.

**Cohort Analysis:**

Create a chart to track weekly revenue per user for each cohort.

Calculate cumulative revenue by summing weekly values.

Compute average cumulative revenue across all cohorts for each week.

**Revenue Prediction:**

- Predict future revenue for 12 weeks using average cumulative growth percentages.
- Generate a chart showing predicted revenue trends for all cohorts.
- Visualization and Insights:
Create charts with conditional formatting to highlight trends and anomalies.
Present actionable insights for improving user retention and maximizing CLV.

**Tools & Technologies**

SQL: Data extraction, transformation, and calculations.
BigQuery: Advanced SQL functionalities, including APPROX_QUANTILES.
Data Visualization: Tableau for creating interactive dashboards.

**Deliverables**

RFM Analysis Output:
Tables for RFM values, RFM quartiles, and RFM scores.
Segmentation dashboard with insights for marketing strategies - Link to RFM Tableau Dashboard: https://public.tableau.com/views/RFMandCustomerSegmentation/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

**CLV Analysis Output:**

Weekly cohort analysis and cumulative revenue charts.

Predicted revenue trends for future cohorts.

Insights & Recommendations

