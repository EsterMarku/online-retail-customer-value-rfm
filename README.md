# Online Retail: Customer Value & RFM Segmentation

**Goal:** Identify which customers and products drive most revenue, and turn that into clear, actionable segments for targeted marketing and retention.

## Dataset

- Source: UCI Machine Learning Repository – Online Retail II  
- Link: http://archive.ics.uci.edu/dataset/502/online+retail+ii  
- Data: Two years of UK-based online retail transactions (invoices, products, quantities, prices, customer IDs).

This repo does **not** include the raw Excel or the cleaned parquet file due to size.  
To reproduce the analysis:

1. Download the dataset from UCI.
2. Place `online_retail_II.xlsx` in a local `data/` folder.
3. Open and run `online_retail_customer_value_rfm_analysis.ipynb`.

The notebook will:
- Load and clean the raw data
- Create a `Revenue` field
- Perform RFM segmentation
- Export the CSV tables and charts in this repo

## Key Insights

- **Top 20% of customers generate ~80% of total revenue**  
  → Strong Pareto / Lorenz effect (see `customer_revenue_pareto.png`)

- **Champions segment**
  - ~800 customers
  - ~63% of total revenue  
  → High priority for VIP treatment, early access and retention programmes

- **At Risk High-Value segment**
  - Smaller share of customers
  - ~12% of revenue at risk  
  → Ideal target for win-back campaigns and time-bound offers

- **Product concentration**
  - A small set of SKUs drives most revenue for Champions and other high-value segments  
  → See `top_products_high_value_customers.png` and `rfm_segment_product_heatmap.png`  
  → Supports SKU prioritisation, inventory planning and targeted promotions

- **Country concentration**
  - UK contributes the vast majority of revenue  
  → `appendix_country_revenue.png` keeps this as an appendix insight

## Files in This Repository

- `online_retail_customer_value_rfm_analysis.ipynb` – full analysis notebook

**Outputs (figures)**  
- `revenue_distribution_client_ready.png` – transaction revenue distribution (log scale)  
- `customer_revenue_pareto.png` – Pareto / Lorenz curve of customer revenue  
- `rfm_segment_overview.png` – customers, revenue and revenue share by segment  
- `rfm_segment_product_heatmap.png` – revenue by RFM segment × top products  
- `top_products_high_value_customers.png` – top SKUs for high-value customers  
- `appendix_country_revenue.png` – high-value revenue by country

**Outputs (tables)**  
- `rfm_customer_segments.csv` – customer-level RFM scores and segment labels  
- `rfm_segment_summary.csv` – segment-level counts and revenue metrics  
- `rfm_segment_product_pivot.csv` – segment × product revenue matrix

## How to Run Locally

1. Create and activate a virtual environment (optional but recommended).
2. Install dependencies (example):

   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
