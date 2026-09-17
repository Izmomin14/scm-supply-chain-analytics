# 🚚 Supply Chain Management (SCM) Analytics

End-to-end data analytics project on a 6-table relational e-commerce supply chain dataset — covering data cleaning and SQL-based analysis to uncover delivery, supplier, inventory, and profitability issues.

---

## 📑 Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Problem Statement](#-problem-statement)
- [Key Findings](#-key-findings)
- [Suggestions](#-suggestions)
- [Tools Used](#-tools-used)
- [About Me](#-about-me)

---

## 📌 Overview

This project analyzes an end-to-end e-commerce supply chain — from **suppliers → inventory → products → orders → customers** — to understand where delivery delays, supplier risk, stockouts, and loss-making orders are coming from. The workflow covers:

1. Raw data cleaning and standardization (Python/Pandas)
2. Building and validating relationships across 6 linked tables
3. SQL-based exploratory analysis (25 queries — easy, medium, and hard)
4. Extracting actionable business insights on delivery, supplier, inventory, and profit performance

---

## 📊 Dataset

- 6 relational tables built from a base e-commerce supply chain dataset, linked via shared keys:
  - **suppliers** — supplier details, country, lead time, rating
  - **inventory** — stock quantity, reorder level, warehouse location, last restocked date (linked to products & suppliers)
  - **products** — product name, category, price, supplier
  - **customers** — customer demographics and location
  - **orders** — order status, delivery status, shipping mode, shipping dates
  - **order_items** — order-level quantity, pricing, discount, profit, and sales
- Data was intentionally kept slightly dirty (nulls, duplicates, inconsistent casing, mixed date formats) to reflect real-world messiness and practice cleaning
- Relationships are realistic — each supplier is tied to specific product categories, mirroring how real procurement works

---

## ❓ Problem Statement

The business lacks clear visibility into how many orders are delivered late, and which shipping mode or region contributes most to delays. Supplier reliability isn't being tracked — it's unclear which suppliers are low-rated or slow. Inventory management is weak, with several products already below reorder level or not restocked in over 60 days. Category and product-level profitability is unclear, and a notable share of orders are loss-making without a known pattern. High-value/repeat customers haven't been identified, the impact of discounts on profit hasn't been validated, and there's no visibility into warehouse-wise stock distribution or sales/profit trends over time.

**Goal:** Clean the data, model it as relational tables, and use SQL to identify delivery bottlenecks, supplier risk, inventory gaps, and profitability drivers across the supply chain.

---

## 🔑 Key Findings

- **53.8% of orders are delivered late** — a major operational red flag
- 2 suppliers (EliteGear Manufacturing, Horizon Retail Supply) have ratings below 3 — risky to depend on
- **14 products** are currently below their reorder level — immediate stockout risk
- **11 products** haven't been restocked in 60+ days — sign of inventory neglect
- **Fishing** is the top revenue and profit-generating category, followed by Cleats and Camping & Hiking
- **18.49% of orders are loss-making** — nearly 1 in 5 orders results in a loss
- Fastest supplier is Bright Path Trading, averaging a 4-day lead time — a strong benchmark for others
- Only 2 customers placed more than 5 orders — repeat-purchase behavior is very low
- Discount rate shows almost no correlation with profit ratio — discounting isn't improving profit margins

---

## 💡 Suggestions

- Investigate root causes of the high late-delivery rate by shipping mode and region
- Review or replace low-rated, unreliable suppliers
- Set up automated reorder alerts for products nearing/below reorder level
- Prioritize restocking for products inactive 60+ days to avoid lost sales
- Double down on high-performing categories (Fishing, Cleats, Camping & Hiking) in marketing/inventory planning
- Audit loss-making orders to identify pricing or discount issues driving negative margins
- Reassess the discount strategy, since it isn't translating into higher profit
- Build a customer loyalty/repeat-purchase program to improve retention

---

## 🛠 Tools Used

- **Python** (pandas) — data cleaning, transformation, and relational table building
- **SQL** — exploratory analysis and business-question querying

---

## 👤 About Me

**Momin Izhar**

**mominn.izhar@gmail.com**
Fresher building a data analytics portfolio through hands-on practice projects using Python and SQL, with a focus on supply chain and BFSI use cases.

📞 9834011201
