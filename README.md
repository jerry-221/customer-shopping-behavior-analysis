# 🛍️ Customer Shopping Behavior Analysis

An end-to-end data analytics project analyzing the shopping behavior of 3,900 retail customers to uncover revenue drivers, identify customer segments, and optimize product strategies.

This project covers the complete data lifecycle: **Python (Data Cleaning & Feature Engineering) ➔ MySQL (Advanced SQL Analysis) ➔ Power BI (Interactive Dashboard).**

---

## 🚀 Project Deliverables (For Recruiters)

*   📊 **[Interactive Power BI Dashboard](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/Customer_Behavior_Dashboard.pbix)** *(Download and open in Power BI Desktop)*
*   💻 **[33 SQL Business Queries](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/queries.sql)**
*   📁 **[SQL Query Results & Screenshots](https://github.com/jerry-221/customer-shopping-behavior-analysis/tree/main/Queries_screenshots)**
*   📓 **[Python Jupyter Notebook](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/Customer_Shopping_Behavior_code.ipynb)**
*   🖼️ **[Dashboard Screenshot](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/Dashboard_Screenshot%202026-11-06%20131744.png)**

---

## 📖 Business Problem
A leading retail company wanted to understand its customers' purchasing patterns across demographics, categories, and sales channels. The objective was to uncover which factors (discounts, reviews, seasons, payment methods) drive consumer decisions and repeat purchases. 

**Core Question:** *How can the company leverage shopping data to identify trends, improve engagement, and optimize product strategies?*

---

## 🛠️ Tech Stack & Workflow

*   **Python (pandas, seaborn):** Handled data cleaning, imputed missing values, and engineered 11 new features.
*   **MySQL:** Stored the cleaned dataset and ran advanced analytical queries.
*   **Power BI:** Built an executive dashboard with interactive slicers, cross-filtering, and KPI cards.
*   **Git/GitHub:** Version control and documentation.

### 1. Data Engineering (Python)
*   **Imputation:** Filled 37 missing `Review Rating` values using category-level medians to prevent demographic bias.
*   **Dimensionality Reduction:** Dropped the redundant `promo_code_used` column after verifying a 100% match with `discount_applied`.
*   **Feature Engineering:** Created 11 new business metrics, including `customer_lifetime_value` (approximate), `loyalty_tier` (New/Returning/Loyal), `region` (mapped 50 states to 4 US regions), and `purchase_frequency_days`.

### 2. Advanced SQL Analytics (MySQL)
Wrote 33 queries ranging from basic descriptive statistics to complex window functions. Key technical highlights include:
*   **Window Functions:** Used `ROW_NUMBER()` to rank products by order volume within their specific category.
*   **CTEs & Self-Joins:** Used Common Table Expressions to calculate product performance vs. overall averages and to identify margin-risk inventory.
*   **Pareto (80/20) Analysis:** Leveraged nested `SUM() OVER()` window functions to calculate the cumulative revenue distribution of the customer base.

---

## 🖥️ Dashboard Preview

![Customer Behavior Dashboard](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/Dashboard_Screenshot%202026-11-06%20131744.png?raw=true)

---

## 💡 Key Business Insights

1.  **The Subscription Paradox:** Non-subscribers account for 73% of the customer base and generate roughly **$170K in revenue**, whereas the 1,053 subscribers generate only **$62K**. Average spend is virtually identical (~$59). The subscription program is failing to upsell customers and needs an incentive revamp.
2.  **Geographic Concentration:** The **South region is the highest revenue driver ($75,275)**, while the Northeast is the lowest ($39,933). Marketing spend should be reallocated toward the South and West regions to maximize ROI.
3.  **Discount Dependency:** Top-selling products like **Sunglasses, Boots, and Hats** show a **44–46% discount application rate**. This indicates a high margin-risk dependency; these items likely struggle to sell at full retail price.
4.  **Demographic Sweet Spot:** **Young Adults (18-28)** and **Middle-Aged** demographics drive the highest revenue (~$60K+ each). Additionally, male customers generate 52% of total revenue but female customers spend slightly more per order on average.
5.  **Payment Preferences:** Digital Wallets (PayPal, Venmo) and Credit Cards dominate, making up the vast majority of transactions, suggesting the checkout UX should be optimized primarily for these digital methods.

---

## 📂 Repository Structure
*   `Customer_Shopping_Behavior_code.ipynb` — Python EDA, data cleaning, and feature engineering.
*   `customer_shopping_behavior.csv` — Raw dataset.
*   `customer_shopping_behavior_clean.csv` — Cleaned, 30-column dataset used for SQL and BI.
*   `queries.sql` — 33 formatted SQL queries with business context.
*   `Queries_screenshots/` — Visual proof of the 8 most impactful SQL results.
*   `Customer_Behavior_Dashboard.pbix` — The interactive Power BI file.
*   `Dashboard_Screenshot 2026-11-06 131744.png` — High-res image of the dashboard.

---
*Created by Pranav Patil*
