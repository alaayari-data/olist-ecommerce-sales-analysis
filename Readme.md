# Olist E-Commerce Sales Analysis

An end-to-end e-commerce data analysis project built on the Brazilian Olist dataset. The goal: turn raw marketplace data into a clean analytical model and a multi-page Power BI dashboard that highlights sales performance, customer behavior, delivery operations, satisfaction, and payment patterns.

## Dataset

The project uses the **Brazilian E-Commerce Public Dataset by Olist**, containing approximately 100,000 orders made between 2016 and 2018.

**Source:** [Kaggle — Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/olistbr/brazilian-ecommerce?trk=article-ssr-frontend-pulse_little-text-block&utm_source=chatgpt.com)

The original dataset contains information about orders, products, customers, sellers, payments, reviews, and delivery performance.

## What's in here

```text
notebooks/      Python exploratory data analysis
powerbi/        Power BI dashboard and related files
screenshots/    Dashboard screenshots
requirements.txt
README.md
```

## Analysis

The project explores the data from several business perspectives:

* **Executive Overview** — revenue, orders, customers, AOV, geography, and delivery performance
* **Sales & Product Performance** — revenue growth, product categories, sales volume, and payment behavior
* **Customer Analysis** — customer distribution, purchase frequency, AOV, and customer concentration
* **Delivery & Operations** — late deliveries, delivery times, delays, and geographic performance
* **Customer Experience & Payments** — review scores, delivery satisfaction, payment methods, and installments

## Key Findings

### 1. Revenue growth was primarily volume-driven

Revenue increased from **R$7.25M in 2017 to R$8.69M in Jan–Aug 2018**, while AOV remained almost flat (**R$160.74 → R$161.04**).

### 2. Customers are highly concentrated geographically

São Paulo accounts for approximately **42% of customers and sales volume**, making it the dominant market. RJ and MG have smaller customer bases but higher AOV.

### 3. Product categories behave differently

`cama_mesa_banho` leads unit sales, while `relogios_presentes` generates similar revenue with significantly fewer units, showing a clear difference between sales volume and revenue contribution.

### 4. Delivery performance affects customer satisfaction

On-time orders average around **4.3/5**, compared with **2.6/5 for late orders** and **1.8/5 for undelivered orders**, showing a strong association between delivery performance and customer satisfaction.

### 5. Payment behavior is highly concentrated

Credit cards account for approximately **79–81% of total payment value**, followed by boleto at around **18–19%**.

## Recommendations

* **Improve customer retention** through loyalty programs and targeted post-purchase offers.
* **Increase AOV** through bundles, cross-selling, and free-shipping thresholds.
* **Investigate high-value markets** such as RJ and MG for further growth opportunities.
* **Prioritize delivery improvements** in states with consistently high late-delivery rates.
* **Monitor payment concentration** while maintaining a smooth credit-card experience.

## Data Limitations

* **2016 has limited activity**, while **2018 covers only January–August**, so year-over-year comparisons should be interpreted cautiously.
* `payment_value` includes freight and therefore should not be interpreted as pure product revenue.
* Customer and order-level analyses use different grains, so measures are calculated at the appropriate level to avoid double counting.

## Dashboard

The final Power BI report contains five pages focused on the main business questions identified during the analysis.

Screenshots of the final dashboard are available in the `screenshots/` folder.

## Tools & Technologies

* **Python** — Data cleaning, transformation, exploratory data analysis, and feature engineering
* **Power BI** — Data modeling, DAX measures, interactive dashboards, and business analysis
* **Pandas** — Data manipulation and analysis

## Project Structure

```text
olist-ecommerce-sales-analysis/
│
├── README.md
├── notebooks/
│   └── Olist_Analysis.ipynb
│
├── powerbi/
│   └── Olist_Dashboard.pbix
│
├── screenshots/
│   ├── overview.png
│   ├── sales_product.png
│   ├── customers.png
│   ├── delivery.png
│   └── customer_experience.png
│
└── requirements.txt

