# Customer Value Segmentation for Marketing Optimisation  
**RFM Analysis | Business-First Customer Analytics**

---

## 📊 At a Glance
- **Data**: ~1M retail transactions over ~2 years  
- **Customers**: Customer-level behavioural aggregation  
- **Segments**: 4 actionable customer groups  
- **Key Insight**: Clear 80/20 revenue concentration  
- **Tools**: Python (pandas, numpy, matplotlib, seaborn), Jupyter  

---

## About This Project
Marketing teams operate with constrained budgets while customer value is **unevenly distributed**.  
This project applies **RFM (Recency, Frequency, Monetary) segmentation** to identify where marketing spend delivers the **highest return** and where resources are diluted across low-value customers.

The objective is **decision support**, not just segmentation by translating customer data into **clear, actionable marketing and retention strategies** under real-world data constraints.

---

## Executive Summary
This project demonstrates an **end-to-end customer analytics workflow** designed to support **marketing spend optimisation and retention prioritisation**.

Using transaction-level retail data, customers are segmented based on purchasing behaviour and mapped directly to **recommended business actions**. The analysis emphasises **commercial reasoning, stakeholder relevance, and honest assumptions**, reflecting how analytics is applied in practice.

---

## Business Problem
Marketing budgets are often allocated uniformly despite large differences in customer value.  
This results in:
- Wasted spend on low-value or dormant customers  
- Under-investment in high-value and at-risk segments  
- Lower overall marketing ROI  

**Key decision question:**  
> *How should a business prioritise customers to maximise customer value and reduce inefficient marketing spend?*

---

## Stakeholder Context
This analysis is designed for:
- Head of Marketing  
- Growth & Retention Managers  
- Commercial / Strategy Teams  

Outputs are framed to support **resource allocation, retention strategy, and campaign prioritisation**.

---

## Methodology Overview
1. **Data Cleaning & Preparation**
   - Transaction-level preprocessing
   - Handling cancellations, missing values, and outliers
   - Customer-level feature engineering  

2. **RFM Feature Construction**
   - **Recency**: Time since last purchase  
   - **Frequency**: Number of purchases  
   - **Monetary**: Total customer spend  

3. **Customer Segmentation**
   - RFM scoring and segmentation logic
   - Distribution analysis and Pareto (80/20) validation  

4. **Decision Translation**
   - Segment-to-action mapping
   - Scenario-based commercial reasoning  

---

## Key Findings
- A **small proportion of customers contributes a disproportionate share of total revenue**, consistent with the Pareto principle.
- High-value and loyal customers justify **retention-focused investment**, while low-value segments present opportunities for **spend reduction or suppression**.
- Without segmentation, marketing spend risks being diluted across customers with vastly different value profiles.

---

## Segment-to-Action Mapping

| Segment | Business Meaning | Recommended Action |
|------|----------------|-------------------|
| Champions | High spend, frequent, recent buyers | Retention incentives, loyalty rewards, early access |
| Loyal Customers | Stable repeat purchasers | Upsell, cross-sell, personalised offers |
| At-Risk High Value | Previously valuable, declining activity | Targeted win-back campaigns |
| Low Value / Dormant | Low spend, infrequent or inactive | Reduce paid marketing, suppress campaigns |

---

## Estimated Commercial Impact (Scenario-Based)
This section illustrates how segmentation supports **more efficient allocation of marketing resources**.

**Assumptions**
- Marketing budget is fixed  
- Customer segments differ significantly in value  
- Some spend is currently allocated to low-value segments  

**Scenario**
If a portion of spend targeting low-value customers is reallocated toward high-value or at-risk segments:
- Retention efficiency is expected to improve  
- Revenue per targeted customer increases  
- Marketing ROI improves through reduced waste  

Misallocating spend toward low-value segments represents an **opportunity cost**, as retention investments typically yield higher marginal returns than acquisition in mature customer bases.

*This project does not estimate exact financial uplift; it demonstrates decision logic and commercial reasoning.*

---

## Visual Outputs
- Customer value distribution charts  
- Segment breakdown visualisations  
- Log-scaled plots for skewed monetary distributions  

All visualisations are designed to be **stakeholder-ready** and suitable for executive presentation.

---

## Limitations & Next Steps
**Limitations**
- No marketing cost or margin data  
- No channel-level attribution  
- No explicit churn labels  

**Next Steps (with additional data)**
- Customer Lifetime Value (CLV) modelling  
- Churn prediction for at-risk segments  
- A/B testing framework for segment-specific campaigns  
- ROI measurement post-implementation  

---

## Portfolio Context
This project represents my approach to **business-first analytics**:
- Translating technical outputs into commercial decisions  
- Designing analysis for stakeholder communication  
- Balancing statistical rigour with practical application  

*See my portfolio for complementary work in predictive modelling and decision-grade dashboards.*

---

## Tools & Technologies
- **Python** (pandas, numpy, matplotlib, seaborn)  
- **Jupyter Notebook**  
- **Parquet** for efficient data storage  

---

## Why This Project Matters
This project demonstrates:
- End-to-end analytical thinking  
- Strong business framing and stakeholder awareness  
- Ability to translate data into **actionable strategy**  
- Professional judgement under real-world data constraints  

It reflects how analytics creates impact **beyond models and charts**.

---

## Author
**Ester Marku**  
MSc Business Analytics  
Customer Analytics • Marketing Optimisation • Data-Driven Decision Making  


