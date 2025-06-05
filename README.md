# 🧠 Customer Segmentation (Python + Power BI | 2025)

📌 **Project Overview**  
This project applies RFM analysis and unsupervised clustering (KMeans) on real-world ecommerce data (Online Retail II), with the goal of segmenting customers based on behavior and visualizing insights using Power BI.

The objective is to showcase end-to-end data storytelling, from cleaning to modeling to dashboard design, simulating how analysts deliver insights for marketing teams or product strategy.

---

## 🔍 Business Questions

- 🧾 Who are our most valuable customers?
- 🧲 How can we identify churn-prone or low-value segments?
- 🛒 Are there clear clusters of behavior based on RFM metrics?
- 📊 How can we visualize customer segments to support targeted campaigns?

---

## 🛠️ Tools Used

| Tool           | Purpose                                  |
|----------------|-------------------------------------------|
| Python         | Data cleaning, feature engineering        |
| Pandas, NumPy  | Data wrangling                            |
| Scikit-learn   | Clustering with KMeans                    |
| Power BI       | Dashboard visualization                   |
| Git & GitHub   | Version control + public portfolio        |

---

## 📊 Project Workflow

### 1. **Data Collection & Cleaning**
- Source: [UCI Online Retail II Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)
- Period: 2010–2011 UK ecommerce transactions
- Removed nulls, returns (invoices starting with "C"), and outliers
- Created `TotalPrice = Quantity * UnitPrice`
- Filtered for `Country = United Kingdom`

### 2. **RFM Feature Engineering**
- Calculated **Recency, Frequency, Monetary** for each customer
- Normalized metrics for modeling

### 3. **Clustering & Insights**
- Applied **KMeans clustering** to RFM data
- Evaluated optimal clusters (Elbow Method + Silhouette Score)
- Interpreted cluster profiles (high-value vs. at-risk, etc.)

### 4. **Dashboard Design (Power BI)**
- Visuals:
  - Cluster summary cards
  - Segment distribution by value
  - RFM distributions per cluster
- Filters:
  - Segment dropdown
  - Monetary range slider

---

## 📈 Final Dashboard

🔗 **Live Dashboard (Power BI)**  
(*Coming soon – link to Power BI Service or screenshot preview*)

📦 **Power BI File (`.pbix`)**  
Located in `powerbi_dashboard/customer_segmentation.pbix`

---

## 🧠 Key Insights

- 🥇 Top cluster: high frequency, high monetary, low recency
- ⚠️ At-risk customers: long recency, low frequency
- 🧬 Clear distinction between 3 core segments
- 📣 Business can tailor marketing to high-value + reactivation targets

---

## 🚀 Future Work

- Add demographic dimensions (if available)
- Deploy dashboard to Power BI service with refresh schedule
- Explore time series patterns by invoice date
- Use DBSCAN or Hierarchical clustering for comparison

---

## 📂 Folder Structure
```
customer-segmentation-analysis/
├── data/
│ ├── raw/
│ └── processed/
├── notebooks/
│ ├── 01_data_cleaning.ipynb
│ ├── 02_rfm_analysis.ipynb
│ └── 03_kmeans_clustering.ipynb
├── powerbi_dashboard/
│ └── customer_segmentation.pbix
├── visuals/
│ └── dashboard_preview.png
└── README.md
```
---
## 📬 Let’s Connect

📫 I'm actively seeking **Data Analyst roles (UK or remote)**.  
More projects: [github.com/Larry0615](https://github.com/Larry0615)

---
