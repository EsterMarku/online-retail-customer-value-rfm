# Online Retail – Customer Value & RFM Segmentation Analysis

## Executive Summary

This project analyses the **UCI Online Retail II dataset** to identify which customers and products drive the majority of revenue in an online retail business. Using descriptive statistics, Pareto analysis, and **RFM (Recency–Frequency–Monetary) segmentation**, the analysis demonstrates how revenue optimisation is driven by **customer and product focus rather than volume growth**.

The results show that transaction values are highly right-skewed and that a small proportion of customers generate a disproportionate share of total revenue. High-value customers concentrate spending on a limited set of products, creating clear opportunities for targeted retention strategies, personalised marketing, and inventory prioritisation.

---

## Business Context

Online retail businesses typically face:
- High customer acquisition costs
- Large product catalogues
- Uneven revenue contribution across customers and products

Understanding **who the most valuable customers are**, **which products they purchase**, and **which segments are at risk** is essential for sustainable revenue growth. This project demonstrates how customer segmentation and revenue concentration analysis can support data-driven commercial decision-making.

---

## Business Questions

1. How is revenue distributed across transactions and customers?
2. Which customer segments contribute the most to total revenue?
3. Which high-value customer segments are at risk of churn?
4. Which products drive revenue among high-value customers?
5. How concentrated is revenue across customers and products?

---

## Dataset

- **Source:** UCI Machine Learning Repository – Online Retail II  
- **Time Period:** 2009–2011  
- **Business Type:** UK-based online retailer  
- **Geographic Scope:** United Kingdom and international customers  

### Key Variables
- Invoice Number  
- Customer ID  
- Invoice Date  
- Quantity  
- Unit Price  
- Country  

---

## Methodology

### Data Preparation
- Removed cancelled and invalid transactions
- Filtered negative quantities and prices
- Calculated transaction-level revenue
- Aggregated customer-level metrics

### Exploratory Data Analysis
- Log-scaled revenue distributions to capture heavy-tailed behaviour
- Compared mean and median transaction values
- Used a Pareto (Lorenz) curve to assess revenue concentration

### RFM Segmentation
Customers were segmented using:
- **Recency:** Days since last purchase  
- **Frequency:** Number of transactions  
- **Monetary:** Total revenue contributed  

Key segments include:
- Champions  
- Loyal High-Value  
- At-Risk High-Value  
- Potential Loyalists  
- Needs Attention  
- Promising  
- New Customers  
- Hibernating  

### Product-Level Analysis
- Revenue by product within each RFM segment
- Identification of top products for high-value customers
- Segment–product revenue heatmap

### Geographic Analysis (Appendix)
- High-value customer revenue by country

---

## Key Insights

- Revenue is **highly concentrated**, with a small proportion of customers generating the majority of total revenue.
- Transaction values are **right-skewed**, where a few large orders disproportionately impact performance.
- **Champions** generate the largest revenue share despite representing a minority of customers.
- **At-Risk High-Value** customers present a significant retention opportunity.
- High-value customers repeatedly purchase a **small set of products**.
- Revenue is predominantly generated in the **United Kingdom**, with smaller international contributions.

---

## Visual Outputs

The project includes:
- Revenue distribution (log scale)
- RFM segment overview (customers, revenue, revenue share)
- RFM segment × product revenue heatmap
- Top products for high-value customers
- Customer revenue Pareto curve
- Geographic revenue breakdown (appendix)

All figures are stored in the `figures/` directory.

---

## Repository Structure

```text
online-retail-customer-value-rfm/
│
├── data/
│   ├── rfm_segment_summary.csv
│   ├── rfm_segment_product_pivot.csv
│   └── rfm_customer_segments.csv
│
├── figures/
│   ├── revenue_distribution.png
│   ├── rfm_segment_overview.png
│   ├── rfm_segment_product_heatmap.png
│   ├── top_products_high_value_customers.png
│   └── customer_revenue_pareto.png
│
├── notebook/
│   └── online_retail_customer_value_rfm_analysis.ipynb
│
└── README.md
