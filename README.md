# Customer Behaviour Analysis

> End-to-end retail data analysis — from raw CSV to SQL insights and Power BI dashboard.

![Python](https://img.shields.io/badge/Python-3.x-blue) ![SQL Server](https://img.shields.io/badge/SQL-Server-teal) ![Power BI](https://img.shields.io/badge/Power-BI-yellow)

## Overview

This project analyses customer purchasing behaviour for a retail/e-commerce business to answer a core business question: how can a company increase revenue, improve customer retention, and optimise marketing strategies?

The dataset contains 5,000 customer transaction records spanning demographics, product categories, payment methods, shipping preferences, discount usage, and review ratings.

## Business Problems Addressed

- Low customer retention — identifying frequent vs one-time buyers
- Ineffective marketing — measuring discount and promo code impact
- Product demand — finding top-revenue categories and products
- Payment behaviour — understanding preferred payment methods
- Seasonal variation — spotting which seasons drive peak sales
- Customer segmentation — grouping into new, returning, and loyal

## Key Findings

| Insight | Result |
|---|---|
| Highest revenue category | Electronics (£486K) |
| Discount impact | Discounted avg spend £219 vs £182 without |
| Top gender revenue | Male (£391K) |
| Subscription effect | Subscribers spend 63% more on average |
| Largest customer segment | Loyal customers (3,085) |
| Top age group by revenue | 51+ age group (£399K) |

## Project Workflow

1. **Data Loading & EDA** — Pandas exploration (shape, dtypes, nulls, statistics)
2. **Data Consistency Check** — corrected mismatched Item ↔ Category mappings
3. **Missing Value Handling** — domain-aware logic per column (e.g. Electronics → "Not Applicable" for size)
4. **Duplicate Removal** — identified and removed using Customer ID
5. **Column Standardisation** — snake_case, lowercase, SQL-friendly naming
6. **SQL Server Export** — via pyodbc and SQLAlchemy
7. **SQL Analysis** — 12 business queries answered
8. **Power BI Dashboard** — interactive filters for Category, Gender, Discount, Subscription

## Tech Stack

- **Python** — Pandas, NumPy
- **SQL** — SQL Server, pyodbc, SQLAlchemy
- **Visualisation** — Power BI

## Dataset Columns

`customer_id` · `age` · `gender` · `item_purchased` · `category` · `purchase_amount` · `location` · `size` · `color` · `season` · `review_rating` · `subscription_status` · `shipping_type` · `discount_applied` · `previous_purchases` · `payment_method` · `frequency_of_purchases`
