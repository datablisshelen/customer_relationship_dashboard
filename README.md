# Credit Card Churn Analysis  
## Relationship Depth & Behavioural Engagement

**Author:** Helen Bliss  
**Project Type:** Hackathon Project – Power BI Analytics  
**Tools:** Power BI, DAX, GitHub

---

**PowerBI dashboard link:** https://app.powerbi.com/links/K7R6jWh5PG?ctid=c233c072-135b-431d-af59-35e05babf941&pbi_source=linkShare

---

## Executive Summary

This project demonstrates how customer churn can be predicted and prevented by focusing on **relationship depth and behavioural disengagement**, rather than contact frequency alone.

By shifting from reactive retention to **behaviour-led early intervention**, the analysis enables the bank to:
- Identify churn risk earlier  
- Target retention resources more precisely  
- Strengthen customer relationships before disengagement becomes irreversible  

The final output is a fully modelled, interactive **Power BI dashboard** designed for business decision-making.

---

## Project Overview

The analysis uses the **Bank Churners** dataset to explore behavioural drivers of customer attrition.

The project delivers:
- A dimensional Power BI data model
- Behavioural segmentation and engineered risk metrics
- Interactive dashboards for insight discovery and prioritisation
- Actionable business recommendations

The dashboard helps stakeholders understand:
1. How relationship depth affects customer stability  
2. How behavioural signals (contact, inactivity, utilisation) predict churn  
3. Which existing customers currently show high-risk patterns  

---

## Role & Responsibilities

As the data analyst on the project, I was responsible for:
- Independent data exploration and hypothesis development  
- Feature engineering and behavioural segmentation  
- Power BI data modelling and DAX metric development  
- Dashboard design with slicers, tooltips, and interactions  
- Translating insights into preventative retention strategies  
- Managing delivery within a fast-paced hackathon environment  

---

## Hypotheses

1. Customers with deeper relationships (more products, longer tenure, higher engagement) have lower churn risk.  
2. Churn risk increases when disengagement indicators accumulate:
   - reduced utilisation  
   - increased inactivity  
   - reactive (late) customer contact  
3. At-risk existing customers can be identified using **behavioural composites**, rather than demographic data alone.

---

## Methodology

1. Audit and clean data for modelling readiness  
2. Perform exploratory behavioural analysis (EDA)  
3. Engineer segmentation features for engagement and depth  
4. Build a dimensional Power BI data model with lookup tables  
5. Develop calculated metrics:
   - Customer Lifecycle Stage  
   - Engagement Depth  
   - Utilisation Tier  
   - Disengagement Indicator  
   - Composite Risk Score  
   - Z-Score Standardised Risk  
6. Design interactive dashboards and slicers  
7. Validate insights against business context  
8. Produce prevention-focused recommendations  

---

## Data Cleaning & Preparation

Key data preparation steps included:
- Removing invalid or duplicate customer records  
- Enforcing numeric formats for inactivity, utilisation, contacts, and products  
- Standardising categorical variables (e.g. Income Category, Card Category)  
- Validating tenure and behavioural ranges  
- Resolving a critical Power BI data-load issue that expanded the dataset from ~700 to **10,127 customers**, significantly improving analytical validity  

---

## Feature Engineering & Segmentation

Segmentation thresholds were chosen based on **behavioural inflection points**, not arbitrary percentiles.

### Customer Lifecycle Stage
- **New:** < 12 months  
- **Growing:** 12–36 months  
- **Settled:** > 36 months  

### Product Depth
- **1–2 products:** Shallow relationship  
- **3+ products:** Stable relationship  

### Engagement Depth
- Low / Medium / High  

### Utilisation Tier
- **No utilisation:** Avg utilisation = 0  
- **Low:** < 0.30  
- **Moderate:** 0.30–0.70  
- **High:** > 0.70  

### Inactivity Risk
- **0–2 months:** Stable  
- **3–4 months:** High-risk tipping point  
- **5+ months:** Persistently elevated risk  

### Composite Risk Metrics
- **Composite Risk Score:** Additive model combining inactivity, utilisation, and spend momentum  
- **Z-Score Risk:** Standardised deviation from population average to highlight outliers  

---

## Dashboard Structure

### Tab 1 – Executive Summary
- Churn by Customer Lifecycle (with disengagement overlay)  
- Churn by Engagement Depth  
- Churn by Utilisation Behaviour  
- Composite Z-Score Risk Heatmap  

### Tab 2 – Product Retention
- Retention by Number of Products  

### Tab 3 – Contact & Inactivity
- Contact Frequency vs Inactivity  

### Tab 4 – Inactivity & Risk
- Churn by Months of Inactivity  

---

## Key Insights

- **Product depth is the strongest retention lever:** churn drops sharply at 3+ products  
- **Contact does not prevent churn — timing does:** late contact is reactive, not protective  
- **Inactivity is the primary early warning signal:** churn accelerates after 3 months  
- **Low engagement drives structural risk** across all segments  
- **Utilisation risk is non-linear:** both no use and very high use increase churn  
- **Composite behavioural risk metrics** clearly identify at-risk existing customers  

---

## Business Recommendations

1. **Deepen relationships early** through targeted multi-product adoption  
2. **Intervene before inactivity reaches 3 months**  
3. **Shift from reactive to preventative contact strategies**  
4. **Prioritise low-engagement customers with utilisation extremes**  
5. **Operationalise lifecycle tiers** (New → Growing → Settled)  
6. **Embed behavioural risk scores into CRM workflows**  
7. **Measure behavioural improvement**, not just churn outcomes  

---

## Future Development

- Build a predictive churn model using train/test splits in Python  
- Integrate predicted churn probabilities back into Power BI  
- Develop a “next best product” recommendation engine  
- Introduce behaviour drift monitoring over time  
- Automate retention triggers within CRM systems  

---


---
