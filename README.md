# Retail Sales Analysis

**A comprehensive analysis of digitized sales data for an independent retail store.**


## Background

An elderly couple operating a brick‑and‑mortar retail store in Swat, Pakistan, maintained paper records of every transaction. To optimize inventory management, identify best-selling products, and gain a better understanding of customer spending patterns, these records were digitized and analyzed using Python and the pandas library.


## Objectives

1. **Import & preprocess** the raw CSV sales data into a pandas DataFrame.  
2. **Explore the dataset** to understand data types, detect outliers, and inspect top transactions.  
3. **Aggregate & summarize** sales by product and by invoice to identify high‑value purchases and customer spending behavior.  
4. **Generate descriptive statistics** on invoice totals and investigate the relationship between units sold and revenue.  
5. **Provide actionable insights** and recommendations to the store owners.


## Data

- **Source:**  
  - `data/sales.csv` (raw transaction log provided by store owners, uploaded to this repository’s `data/` folder)

- **Description:**  

  | Column           | Type    | Description                                                      |
  |------------------|---------|------------------------------------------------------------------|
  | `invoice_id`     | int64   | Unique identifier for each sale; repeats for multi‑item invoices |
  | `date`           | object  | Date of the transaction (YYYY‑MM‑DD)                             |
  | `day_of_week`    | object  | Day name (Monday–Saturday)                                       |
  | `product_name`   | object  | Description of the item sold                                     |
  | `units_sold`     | int64   | Quantity of the item sold in that line                           |
  | `price_per_unit` | float64 | Unit price charged                                               |
  | `amount`         | float64 | Line total (units_sold × price_per_unit)                         |


## Environment

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/retail‑sales‑analysis.git
   cd retail‑sales‑analysis


## Key Findings

- **Highest single‑line sale:** A vintage kitchen cabinet sold for $ 295.00 in one invoice.  
- **Top‑selling product by frequency:** “HAND WARMER BIRD DESIGN” appeared on 8 invoices, with 14 units sold in total.  
- **Customer spending behavior (invoices 21–60):**  
  - Mean invoice total: $ 52.55  
  - Maximum invoice total: $ 295.00  
  - Total revenue: $ 2,102.03  
- **Units‑to‑revenue relationship:** Moderate positive correlation (r ≈ 0.62), indicating larger orders tend to generate proportionally higher revenue.  

### Recommendations

1. **Stock up** on hand warmers and 3‑tier cake tins—top revenue generators.  
2. **Bundle promotions** around frequently co‑purchased items (e.g., hand warmers + seasonal décor).  
3. **Monitor low‑cost items** for volume trends to decide whether to expand or phase out offerings.  
