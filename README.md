# Online Retail Customer Value Analysis (RFM Segmentation)

## Overview
This project analyses transactional data from a UK-based online retailer to identify **which customers and products drive the majority of revenue**. Using **RFM (Recency, Frequency, Monetary) segmentation**, revenue concentration (Pareto/Lorenz), and product contribution analysis, the workflow converts raw invoice-level data into **actionable customer segments** for targeted marketing, retention, and inventory decisions.

The analysis shows that revenue is **highly concentrated**: a relatively small share of customers and products accounts for a disproportionate share of total sales.

---

## Dataset
**Source:** UCI Machine Learning Repository — *Online Retail II*  
**Link:** http://archive.ics.uci.edu/dataset/502/online+retail+ii  

**Description:**  
Two years of UK-based online retail transaction data, including invoices, products, quantities, prices, and customer identifiers.

> **Note on data files:**  
> The raw Excel file is **not included in this repository** due to file size constraints. All results are fully reproducible using the publicly available dataset via the link above.

---

## Key Outputs

### Figures (`reports/figures/`)
- `revenue_distribution_client_ready.png` — Transaction revenue distribution (log scale)
- `customer_revenue_pareto.png` — Customer revenue concentration (Pareto/Lorenz curve)
- `rfm_segment_overview.png` — Customers, revenue, and revenue share by segment
- `rfm_segment_product_heatmap.png` — Revenue by RFM segment × top products
- `top_products_high_value_customers.png` — Top products for high-value customers
- `appendix_country_revenue.png` — High-value customer revenue by country (appendix)

### Tables (`outputs/tables/`)
- `rfm_customer_segments.csv` — Customer-level RFM scores and segment labels
- `rfm_segment_summary.csv` — Segment-level customer counts and revenue metrics
- `rfm_segment_product_pivot.csv` — Revenue by RFM segment × product matrix

---

## Reproducibility (Jupyter Notebook)

This analysis was conducted using **Python in Jupyter Notebook**.

### How to run locally
1. Download the dataset from the UCI link above.
2. Place the Excel file locally at:
   ```text
   data/raw/online_retail_II.xlsx
````

3. Open the notebook:

   ```text
   notebooks/online_retail_customer_value_rfm_analysis.ipynb
   ```
4. Run all cells from top to bottom.

The notebook performs:

* Data cleaning and validation
* Revenue calculation (Quantity × Price)
* RFM scoring and segmentation
* Export of all figures and summary tables included in this repository

---

Tools & Skills Demonstrated

* Python (pandas, numpy, matplotlib, seaborn)
* Jupyter Notebook
* Customer analytics & RFM segmentation
* Revenue concentration analysis (Pareto / Lorenz)
* Business-focused data visualisation
* Translating transactional data into strategic insights

---

Author

Ester Marku
MSc Business Analytics
