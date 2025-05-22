# Global Product Inventory Optimization

This repository contains the final project for MGMT 59000 - CFA Spring 2025, where we apply a range of analytical techniques to extract insights from the **Global Product Inventory Dataset 2025**, sourced from Kaggle.

## 📊 Objective

To analyze a realistic e-commerce product catalog and deliver business insights that improve:
- Inventory management
- Product bundling strategies
- Demand forecasting
- Shipment optimization

## 📁 Files Included

- `CFA_FinalProject_aggar158.ipynb`  
  Main analysis notebook implementing EDA, clustering, optimization, and predictive models.

- `products.csv`  
  The dataset used (sourced from Kaggle): [Global Product Inventory Dataset 2025](https://www.kaggle.com/datasets/keyushnisar/global-product-inventory-dataset-2025)

- `Project Proposal.pdf`  
  Project scope, methodology, and early insights submitted for approval.

---

## 🔍 Key Insights

### 🔗 Insight 1: Clustering Based on Shared Tags
- Built an undirected graph to group products using shared tags.
- 6,310 clusters identified; largest includes laptops, smartphones, monitors.

### 🧩 Insight 2: Suggest Complementary Product Bundles
- Used Jaccard similarity to find product pairs ideal for bundling.
- Pairs like Monitor + Smartphone show strong tag overlap.

### 📈 Insight 3: Predict Daily Demand
- Linear regression on price, ratings, warranty, and expiration features.
- Key finding: Demand decreases with price and shorter shelf life.

### 📦 Insight 4: Optimize Restocking Decisions
- Used dynamic programming to weigh cost of holding vs. discarding.
- Identified 32% of products that should be cleared early to avoid loss.

### 🔁 Insight 5: Monthly Replenishment Simulation
- Rolling horizon inventory simulation for 6 months.
- Tracked when to replenish based on forecasted demand.

### 📐 Insight 6: Shipment Volume Optimization
- Integer Linear Program to minimize shipment volume while ensuring diversity.
- Selected 100 units from 3 categories using high-rated, small-volume products.

### 🎯 Insight 7: Maximize Ratings within Shipment Constraints
- 0-1 Knapsack optimization to pack highest-rated products under a 300,000 cm³ limit.

### 🤖 Insight 8: Predict Product Ratings
- Decision Tree Regressor on price, category, and warranty.
- Price is the dominant feature, with MAE ~1.2.

### ⚠️ Insight 9: Flag High-Demand, Low-Rated Products
- Found >10 products with high demand but ratings ≤ 2.5.
- Indicates urgent need for quality improvement or rebranding.

---

## 📚 Tools & Techniques
- Python, pandas, matplotlib, seaborn
- Linear Regression, Decision Tree, Jaccard Similarity
- NetworkX for clustering
- Integer Programming (PuLP)
- Feature Engineering & One-Hot Encoding

---

## 👥 Team Members
- Muskan Aggarwal  
- Deepak Saini  
- Rupali Kakadia  
- Shashank Sridhar

---

## 📌 Course Info
MGMT 59000 – Computational Financial Analytics  
Purdue University, Spring 2025

---
