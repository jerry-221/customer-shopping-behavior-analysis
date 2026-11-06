# 🛍️ Customer Shopping Behavior Analysis

An end-to-end data analytics project analyzing the shopping behavior of 3,900 retail customers. The goal is to uncover revenue drivers, identify customer segments, and optimize product and marketing strategies.

This project covers the complete data lifecycle: **Python (Data Cleaning & Feature Engineering) ➔ MySQL (Advanced SQL Analysis) ➔ Power BI (Interactive Dashboard) ➔ Reporting.**

---

## 🚀 Quick Links (For Recruiters)
*Skip the code and go straight to the deliverables:*

*   📊 **[View the Power BI Dashboard File (.pbix)](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/Customer_Behavior_Dashboard.pbix)**
*   💻 **[Read the 33 SQL Business Queries](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/queries.sql)**
*   📓 **[View the Python Jupyter Notebook](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/Customer_Shopping_Behavior_code.ipynb)**
*   📁 **[Download the Cleaned Dataset](https://github.com/jerry-221/customer-shopping-behavior-analysis/blob/main/customer_shopping_behavior_clean.csv)**
*   📄 *Project Report (PDF) and Presentation Deck (PDF) — [Coming Soon]*

---

## 📖 Project Overview
A leading retail company wanted to better understand its customers to improve sales, satisfaction, and loyalty. Management needed to know which factors—such as discounts, reviews, seasons, or payment preferences—drive consumer decisions and repeat purchases. 

**Core Business Question:** *How can the company leverage customer shopping data to identify trends, improve engagement, and optimize marketing and product strategies?*

---

## 🗂️ Dataset
*   **Source:** `customer_shopping_behavior.csv`
*   **Size:** 3,900 rows, 18 initial columns.
*   **Attributes:** Customer demographics (Age, Gender, Location), purchase details (Item, Category, Amount), and behavioral metrics (Review Rating, Subscription Status, Payment Method, Purchase Frequency).
*   *Note: A cleaned version with 30 columns (including engineered features) is also included in the repository.*

---

## 🛠️ Tools & Technologies
*   **Python (Jupyter Notebook):** `pandas`, `matplotlib`, `seaborn` for EDA, data cleaning, and feature engineering.
*   **SQL (MySQL):** Database storage and advanced analytical querying (CTEs, Window Functions).
*   **Power BI:** Interactive dashboard design and data visualization.
*   **Gamma:** AI-assisted presentation deck creation.

---

## ⚙️ Project Steps

1.  **Data Cleaning & EDA (Python):**
    *   Handled missing values by imputing 37 null `Review Rating` values using category-level medians.
    *   Dropped redundant columns (verified `promo_code_used` was 100% identical to `discount_applied`).
    *   Standardized column names to `snake_case`.
2.  **Feature Engineering (Python):**
    *   Created 11 new features including: `customer_lifetime_value`, `loyalty_tier` (New/Returning/Loyal), `region` (50 states to 4 regions), `payment_category`, and `purchase_frequency_days`.
3.  **Database & SQL Analysis (MySQL):**
    *   Exported the cleaned dataset to a MySQL database.
    *   Wrote **33 business queries** ranging from basic aggregations to advanced analytics (using `ROW_NUMBER()`, `NTILE()`, and `CASE` statements) to extract insights.
4.  **Data Visualization (Power BI):**
    *   Connected Power BI directly to the SQL database.
    *   Built a fully interactive executive dashboard with cross-filtering slicers, KPI cards, and demographic breakdowns.

---

## 🖥️ Dashboard Preview

<img width="1327" height="732" alt="Screenshot 2026-11-06 131744" src="https://github.com/user-attachments/assets/f6718248-04ab-4b3c-8d7a-ca383a3fa8bd" />


![Customer Behavior Dashboard](dashboard_screenshot.png)

---

## 💡 Key Results & Insights

1.  **The Subscription Gap:** Non-subscribers generate 4× the total revenue of subscribers and have a slightly higher average spend. The subscription program is currently attracting lower-value customers.
2.  **Discount Dependency:** 5 specific products (e.g., Sunglasses, Boots, Hats) show ~45% discount rates. These pose a margin risk as they only sell when heavily discounted.
3.  **Geographic & Age Concentrations:** Young adults (18-28) and Middle-aged customers drive the highest total revenue. [Insert your top region insight here, e.g., The South generates X% of revenue].
4.  **Quality Risks:** [Insert your best insight from Q15 here, e.g., "Product X generates high revenue but has a low average rating, posing a reputation risk."]

---

## 🚀 How to Run / View This Project

**To view the Python Notebook:**
1. Click the `.ipynb` file in this repository (or view it directly on GitHub).
2. Alternatively, download the file and open it in Jupyter Notebook or VS Code.

**To run the SQL Queries:**
1. Open your preferred SQL client (MySQL Workbench, PostgreSQL, etc.).
2. Import the `customer_shopping_behavior_clean.csv` file into a new database.
3. Open `queries.sql` and run the queries against the table.

**To view the Power BI Dashboard:**
1. Download the `Customer_Behavior_Dashboard.pbix` file.
2. Open it using **Power BI Desktop** (free download from Microsoft).

---
*Created by [Your Name] — [Link to your LinkedIn Profile]*
