# 🧠 Customer Segmentation (Python + Power BI | 2025)

📌 **Project Overview**  
This project applies RFM analysis and unsupervised machine learning (KMeans clustering ) on real-world ecommerce data (Online Retail II), with the goal of segmenting customers based on behavior and visualizing insights using Power BI.

The objective is to showcase end-to-end customer segmentation pipeline, from cleaning to modeling to dashboard design, simulating how analysts deliver insights for marketing teams or product strategy.

---

## 🔍 Business Questions

- 🧾 Who are our most valuable customers?
- 🧲 How can we identify customers at risk of churning?
- 🧬 Can we group customers into distinct behavioral clusters?
- 📣 How can we tailor marketing actions based on customer types?

---

## 🛠️ Tools Used

| Tool           | Purpose                                  |
|----------------|-------------------------------------------|
| Python         | Data cleaning, feature engineering        |
| Pandas, NumPy  | Data wrangling                            |
| Matplotlib     | Exploratory data visualization            |
| Scikit-learn   | Clustering with KMeans, Silhouette scoring|
| Power BI       | Dashboard visualization                   |
| Git & GitHub   | Version control + public portfolio        |

---

## 📊 Project Workflow

### 1. **Data Collection**
- Source: [UCI Online Retail II Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)
- Period: 2010–2011 UK ecommerce transactions

### 2. 📥 Data Cleaning & Preparation
- Loaded raw Excel 2010–2011 **UK-based online retail transactions**
- Removed:
  - Canceled orders (`InvoiceNo` starting with `'C'`)
  - Nulls and duplicates
  - Non-positive quantities or prices
- Created:
  - `TotalPrice = Quantity * UnitPrice`
- Assigned:
  - `CustomerID` as unique identifier
- Filtered:
  - `Country = United Kingdom`

### 3. 🧮 RFM Feature Engineering
- Calculated:
  - **Recency**: Days since last purchase
  - **Frequency**: Number of purchases
  - **Monetary**: Total amount spent
- Used reference date of `Dec 9, 2011`
- Applied **StandardScaler** for normalization

### 4. 🤖 Unsupervised Clustering (KMeans)
- Applied **KMeans clustering** to RFM data
- Used **Elbow Method** to find optimal cluster count (k=4)
- Verified cluster quality with **Silhouette Score**
- Assigned cluster labels(0,1,2,3) to customer profiles
- Generated final labeled dataset: `rfm_with_segments.csv`

### 5. 📊 Power BI Dashboard
- Imported final dataset and built:
  - 📈 **Bar chart**: Customer count by segment
  - 📌 **KPI Cards**: Avg. Recency (days), Frequency (orders), Monetary (£)
  - 🎨 Color-coded segments for visual clarity
  - 🎛️ Dropdown filter for customer segments
- Dashboard title, tooltips, and custom formatting added
- Saved `.pbix` file for reproducibility

---

## 🧠 Final Customer Segments

| Segment Label        | Description                                               |
|----------------------|-----------------------------------------------------------|
| **Champion**         | Recent, frequent, and high spenders (top 1%)              |
| **Loyal**            | Regular repeat customers with decent monetary value       |
| **Potential Loyalist** | Moderate recency/frequency, high growth potential       |
| **Churn Risk**       | Long inactive, low value — may require reactivation       |

---

## 📊 Dashboard Preview

📦 **Power BI File (`.pbix`)**  
Located at: `powerbi_dashboard/customer_segmentation.pbix`

🖼️ **Screenshot Preview**  
Available in `/visuals/dashboard_preview.png`

> ⚠️ Currently not published online due to Power BI Service limitations with personal accounts. All assets available locally in this repo.

---

## 📌 Key Takeaways

- 🏆 Cluster 2 (Champions) spends **£71,000+** with **60+ orders**
- 📉 Cluster 0 (Churn Risk) has **low frequency & high recency**
- 🔍 RFM segmentation enables **personalized campaigns** and **Customer Lifetime Value(LTV targeting)**
- 🎯 The dashboard simulates deliverables expected in real-world analyst roles

---

## 🚀 Future Enhancements

- Connect to live data and deploy to Power BI Service (when eligible)
- Apply alternative clustering methods: **DBSCAN**, **Hierarchical**
- Combine RFM with demographics or product-level features
- Use DAX measures for dynamic aggregation and drilldowns

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
│ └── dashboard_snapshot.png
└── README.md
```
---
## 💼 About Me

📫 I'm **Olanrewaju Oyenekan**, actively seeking **Data Analyst roles (UK or remote)**.  
This project reflects my capabilities in:
- Data wrangling & modeling
- Clustering algorithms & EDA
- Storytelling with visual tools (Power BI, Tableau)

🔗 [GitHub Portfolio](https://github.com/Larry0615)

---

