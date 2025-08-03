# 🛒 Sprint 2: Instacart Customer Behavior Analysis

## 📁 Project Overview

This project explores Instacart’s 2017 anonymized order data to understand **customer purchasing behavior**, including **when** customers shop, **how frequently** they order, **what products** are popular, and **how much** they typically buy. The dataset was sourced from [Kaggle’s Instacart Market Basket Analysis](https://www.kaggle.com/c/instacart-market-basket-analysis/data).

The goal is to generate **actionable insights** that stakeholders at Instacart (or similar companies) could use to improve marketing, inventory planning, and customer retention.

---

## 📦 Datasets Used

All datasets were loaded from the `/datasets/` directory and include:

- `orders.csv`: Information about customer orders, including time and sequence.
- `products.csv`: Product details such as name and department.
- `departments.csv`: Department IDs and names.
- `aisles.csv`: Aisle IDs and names.
- `order_products.csv`: Information on products included in each order.

---

## 🔧 Cleaning & Preparation

- **Missing values** in `days_since_prior_order` and `product_name` were addressed:
  - Filled missing `product_name` values (only found in aisle 100 / department 21) with `"Unknown"`.
  - Filled missing `add_to_cart_order` values with `999` and cast the column as `int`.
- **Duplicate rows** were identified and removed in the `orders` dataset.
- All categorical and numeric values were validated (e.g., `order_hour_of_day` in 0–23, `order_dow` in 0–6).

---

## 📊 Key Insights

### A. Easy-Level Analysis
- ✅ Most orders occur between **8:00 AM and 6:00 PM**, peaking around midday.
- ✅ **Sunday and Monday** are the most popular shopping days.
- ✅ Many customers reorder after **2–10 days**, with a noticeable bump at **30 days**, likely tied to monthly routines.

### B. Medium-Level Analysis
- ✅ Ordering patterns on **Wednesday vs Saturday** show similar peak hours, but **Saturday** has slightly higher order volume.
- ✅ Most customers place **fewer than 5 orders**, but some are highly loyal with 20+.
- ✅ Top 20 most popular products include **bananas**, **strawberries**, and **whole milk**.

### C. Hard-Level Analysis
- ✅ Most orders contain **5 to 15 items**, averaging **~10 items** per order.
- ✅ The top reordered products reveal strong **brand loyalty** and repeated purchasing of staple items.

---

## 📈 Visualizations

Matplotlib was used to create:
- Bar charts of order frequency by hour and day
- Histograms of time between orders and items per order
- Side-by-side comparisons of order behavior across weekdays

All visuals are clean, stakeholder-ready, and explained with markdown commentary in the notebook.

---

## 🧠 Business Recommendations

- 📆 Focus promotions on **Sunday and Monday** when traffic is highest.
- 🔁 Use personalized emails or app notifications to remind users to reorder around the **5–10 day mark**.
- ⭐ Promote and recommend **popular staple items** based on reorder likelihood.
- 📊 Optimize warehouse and staffing levels based on **peak order hours (8–18)** and **Saturday activity**.

---

## 🛠️ Tech Stack

- **Python** (Pandas, Matplotlib)
- **Jupyter Notebook**
- **CSV data files** from Kaggle
- Local analysis (no database or web integration required)

---

## ✅ How to Run

1. Clone the repository or open the Jupyter notebook in your local environment.
2. Ensure datasets are located in the `/datasets/` folder.
3. Run each notebook cell in order to clean, explore, and visualize the data.
4. Review plots and summaries in markdown cells for insights.

---

## 📚 Credits

- Dataset: [Instacart Market Basket Analysis - Kaggle](https://www.kaggle.com/c/instacart-market-basket-analysis)
- Analysis: Completed as part of a data science project to explore real-world business intelligence use cases.

---

## 📌 License

This project is for educational and non-commercial use only. All data belongs to Instacart and was shared publicly for analysis purposes via Kaggle.
