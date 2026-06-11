# CUSTOMER-ANALYSIS-SQL-DRIVEN-RETENTION-STRATEGY
<img width="1376" height="772" alt="image" src="https://github.com/user-attachments/assets/2fa89bad-b604-4d44-ac79-619f0f27880e" />
# Decoding Customer Value: A SQL-Driven Retention Strategy
IIT Guwahati — Consulting & Analytics Club | Summer Projects '26

## Project Overview
This project analyzes behavioral and transactional data of 3,900 customers 
of a D2C fashion brand to answer one core strategic question:
"Is the business building a loyal customer base, or is it reliant on 
continuous promotional activity to drive revenue?"
---
## Deliverables
| Deliverable | File | Description |
|-------------|------|-------------|
| Python | feature_engineered.csv | Cleaned dataset with 7 engineered features |
| SQL | SQL_Queries.sql | 5 segmentation queries answering all key questions |
| Power BI | Dashboard.pbix | Four-panel founder dashboard |
| Playbook | Retention_Playbook.docx | Promo sunset plan + ideal customer profile |
| Summary | Customer_Intelligence_Report.docx | Executive summary of findings |



## Tech Stack

- Python (Pandas, NumPy) — data cleaning and feature engineering
- SQLite (via Google Colab) — customer segmentation queries
- Power BI Desktop — founder dashboard
- Microsoft Word — playbook and executive summary


## Engineered Features
| Feature | Logic | Business Question Answered |
|---------|-------|---------------------------|
| promo_dependency_score | (Discount Applied + Promo Code Used) / 2 | Does this customer only buy on discount? |
| value_tier | pd.qcut on Purchase Amount — Low/Mid/High | What is this customer's revenue contribution? |
| satisfaction_flag | Review Rating >= 4.0 | Is this customer happy enough to return? |
| loyal_def1 | High prev purchases + low promo dependency | Organically retained customer? |
| loyal_def2 | High value tier + satisfaction flag | Retained by experience, not deals? |
| spend_per_purchase_history | Purchase Amount / (Previous Purchases + 1) | Spending efficiency over time |
| is_subscriber | Subscription Status == Yes | Brand commitment indicator |


## Key Findings
1. 43% of customers (1,700) are fully discount-dependent
2. Organically loyal customers spend 25% more and have 52% more 
   previous purchases than discount-dependent ones
3. No geography shows high spend + low promo dependency simultaneously
   — discount reliance is a systemic brand issue, not regional
4. The brand's ideal customer (562 exist today): Male, age 27-55, 
   Outerwear/Footwear preference, avg spend $93, zero promo dependency

---
## Strategic Recommendations
1. Promotional Sunset: Freeze discounts for ~560 Mid-value 
   discount-dependent customers over 6 months. 
   Target: maintain >70% purchase rate, achieve +15-20% revenue per customer.
2. Acquisition Retargeting: Shift paid campaigns to target the ideal 
   customer profile — male, 27-55, Outerwear/Footwear, 
   Virginia/Vermont/Arizona locations.

## Contact
Ayushi Singh
NITC
ayushi_b240542me@nitc.ac.in
