# Netflix-Customer-Churn-and-Engagement-Analysis
## Analysis of Netflix customer churn.
An end-to-end exploratory analysis of 5,000 Netflix subscribers, built with Power Query and using power BI and creating Dax measures, to understand which customer characteristics and engagement behaviours are linked to churn.
### Project overview 
Project Overview
This project analysed **5,000 Netflix subscribers** to uncover the customer
characteristics and engagement behaviours linked to churn. Data was cleaned
in **Power Query**, measures were built with **DAX**, and an interactive
**Power BI** dashboard was created with KPI cards, charts and slicers.
The analysis found that churn is driven by behaviour rather than demographics:
inactivity, low watch time, the Basic plan, and Crypto or Gift Card payments
are the strongest warning signs
Problem Statement
 What customer characteristics and engagement behaviours are associated with higher churn, and how can Netflix use these insights to better understand and monitor customer retention?
## Data Sources 
**Source:** [Kaggle] Neflix dataset.Microsoft csv file 
- **Size:** 5,000 rows, 14 original columns, plus 4 columns added during analysis
- **Contents:** customer demographics (age, gender, region), subscription type and monthly fee, watch hours, device, payment method, favourite genre, last login days, and churn status

## Tools
Power Query (cleaning) · Power BI (visualisation) · DAX (measures) · Exploratory Data Analysis (descriptive, comparative, engagement and segmentation analysis)

## Data cleaning and preparation
1. Checked all 5,000 rows for exact duplicates: none found. Customer IDs are unique.
2. Checked categorical fields (region, gender, subscription type, device, payment method, favourite genre) for consistency.
3. Validated and assigned correct data types to numeric, categorical and ID columns.
4. Standardised column names and organised fields for analysis.
5. Created **Age Category** (Adult, Middle-Aged Adult, Older Adult).
6. Created churn status, churned category and customer satisfaction score fields.

   ## DAX Measures
Custom measures built for dynamic calculations: Total Customers, Active Members, Churn Rate, Total Churned Customers, Age Category, Churned Category and Satisfaction Score.

## Dashboard Features
- KPI cards for subscribers, churn rate, churned customers, average watch hours and average last login days
- Average watch hours by subscription type vs churn rate (combo chart)
- Churned vs active members (donut chart)
- Churn rate by device, region and favourite genre
- Average monthly fee by subscription type
- Interactive slicers for **Age Category**, **Subscription Type** and **Region**



## Key Findings
- **Inactivity is the top warning sign.** Customers 30+ days since last login churn at about 75%, versus about 13% for those active in the last 7 days.
- **Basic plan churns most:** Basic 61.8%, Standard 45.4%, Premium 43.7%.
- **Low engagement drives churn.** The lowest-viewing fifth of customers churns at 86% versus 8% for the top fifth.
- **Payment method matters.** Crypto (59.7%) and Gift Card (57.8%) users churn far more than Credit/Debit Card (about 44%) and PayPal (47%) users.
- **More profiles, less churn.** Accounts with 4 to 5 profiles churn at 38 to 41%, versus 57 to 59% for 1 to 3 profiles.
- **Churn is behaviour-driven, not demographic.** Device and region differences are small (all roughly 49 to 52%).
- Churned customers represent about **$33.0K of $68.4K** in monthly fees (48%).

## Insight | Recommendation 
- **R1** Churn jumps from 32% to 75% after 30 days of inactivity | Trigger re-engagement emails/push notifications at 14 days of inactivity 
- **R2** Basic churns at 61.8% vs 45.4% for Standard | Offer Basic users upgrade trials and extra perks 
-  **R3** Crypto and Gift Card users churn at 58 to 60% | Nudge them toward recurring card or PayPal payments 
- **R4** Lowest-viewing fifth churns at 86% | Personalised picks during onboarding to drive early viewing 
- **R5** 4 to 5 profile accounts churn about 19 points less | Encourage household-style profile sharing 

## Limitations
- The data is a public Kaggle dataset, so findings may not reflect real Netflix behaviour.
- The analysis is exploratory and shows association, not causation. No predictive model was built.
