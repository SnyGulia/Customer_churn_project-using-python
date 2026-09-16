# Customer_churn_project-using-python
📌 Project Overview

Customer churn is a critical business challenge that directly impacts revenue, growth, and customer lifetime value.

This project analyzes customer, subscription, and support data stored in a SQLite database to uncover churn patterns, evaluate customer retention, and understand the potential revenue impact of customer cancellations.

The analysis follows a complete data analytics workflow—from data extraction and cleaning to feature engineering, KPI calculation, and visualization.

🎯 Project Objectives
📉 Measure overall customer churn and retention.
📦 Compare churn rates across subscription plans.
🌍 Analyze churn patterns across different states.
💰 Calculate Average Revenue Per User (ARPU).
⏳ Evaluate average customer tenure.
🚨 Estimate monthly revenue associated with churned customers.
🎧 Analyze customer complaints and escalation rates.
🔍 Explore relationships between customer and subscription attributes.
📊 Generate meaningful visualizations for business analysis.
🛠️ Technologies & Tools
Technology	Purpose
🐍 Python	Core programming language
🗄️ SQLite	Database storage and querying
🐼 Pandas	Data cleaning, transformation, and analysis
🔢 NumPy	Numerical operations
📈 Matplotlib	Data visualization
🎨 Seaborn	Statistical visualization
📓 Jupyter Notebook	Interactive analysis environment


🔄 Project Workflow
🗄️ SQLite Database
        ↓
📥 Data Extraction
        ↓
🧹 Data Cleaning & Standardization
        ↓
🧩 Feature Engineering
        ↓
🔗 Dataset Integration
        ↓
📊 KPI Calculation
        ↓
📈 Exploratory Data Analysis
        ↓
💡 Business Insights
        ↓
📄 Export Processed Dataset
🧹 Data Preparation

The project performs several data-cleaning and transformation steps:

Renames customer-related columns for consistency.
Removes unnecessary columns from the analysis.
Converts date columns into appropriate datetime formats.
Standardizes gender values.
Handles missing country values using state–country mappings.
Removes unnecessary support-data columns.
Creates a churn indicator using cancellation dates.
Aggregates customer complaint records.
Retains the latest support record for each customer.
🧩 Feature Engineering

The following analytical features are created:

Feature	Description
churn_flag	Indicates whether a customer has churned
complaint_count	Number of support records associated with a customer
tenure_days	Customer subscription duration in days
monthly_charges	Recurring monthly subscription charges
escalated	Indicates whether a support issue was escalated
Churn Definition

A customer is considered churned when a cancellation date is present.

churn_flag = 1 if cancellation_date exists else 0
📊 Key Performance Indicators

The notebook calculates several business-focused metrics:

KPI	Business Meaning
📉 Churn Rate	Percentage of customers who discontinued their subscriptions
🔄 Retention Rate	Percentage of customers who remain active
📦 Churn by Plan	Identifies differences in churn across subscription plans
🌍 Churn by State	Highlights geographic churn patterns
💰 ARPU	Average monthly revenue generated per customer
⏳ Average Tenure	Measures how long customers remain subscribed
💸 Revenue Risk	Monthly charges associated with churned customers
🚨 Escalation Rate	Percentage of support records marked as escalated
🎧 Average Complaint Count	Average number of complaints per customer
📈 Visualizations

The project generates visualizations to support exploratory analysis, including:

📅 Monthly Churn Trend

Examines how customer churn changes over time.

📦 Churn by Subscription Plan

Compares churn across different subscription plans.

🌍 Churn by State

Explores geographic differences in customer churn.

🔥 Correlation Heatmap

Visualizes relationships between selected numerical and encoded variables.

🔍 Pairplot Analysis

Provides a pairwise view of selected customer and subscription attributes.

💡 Business Questions Explored

This project helps investigate questions such as:

Which subscription plans experience higher churn?
How does churn vary across states?
What percentage of customers are retained?
How long do customers typically remain subscribed?
How much recurring monthly revenue is associated with churned customers?
Do customer complaints appear alongside churn patterns?
Which variables may deserve further investigation?

<img width="782" height="657" alt="Screenshot 2026-09-16 213525" src="https://github.com/user-attachments/assets/1055b0d5-ba08-4543-929c-1eaa5abcbf4c" />
<img width="892" height="676" alt="Screenshot 2026-09-16 213454" src="https://github.com/user-attachments/assets/373963e0-a1b0-4dc8-8a41-8bca5214eb3f" />
