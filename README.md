# 👥 Customer Segmentation with K-Means

> Customer segmentation project using unsupervised machine learning — from raw customer data to K-Means clusters, business segment interpretation, and Power BI dashboard.

---

## 📌 Overview

This project focuses on customer segmentation using behavioral, demographic, and financial data. The goal is to group customers into meaningful segments, understand their purchasing behavior, and provide actionable marketing recommendations for each group.

The project uses **K-Means clustering** to identify customer groups based on features such as income, spending score, purchase frequency, loyalty years, online activity, and returns rate.

---

## 📂 Project Structure

```text
customer-segmentation/
├── data/
│   └── customer_data.csv                  # Customer data — demographics, income, spending, loyalty, returns
├── customer_segmentation.ipynb            # Full analysis and clustering pipeline
├── customer_segments.csv                  # Final dataset with assigned customer segments
├── segment_summary.csv                    # Segment-level summary for business analysis
├── customer_segmentation.pbix   # Power BI dashboard
└── README.md
```

---

## 🔍 Analysis Pipeline

**1. Data Loading & Inspection** — shape, dtypes, statistical summary, missing values, duplicates

**2. Feature Selection**
- Selected numerical customer features for clustering
- Used behavioral, financial, loyalty, and return-related variables
- Main features: `age`, `annual_income`, `spending_score`, `purchase_freq`, `avg_order_value`, `loyalty_years`, `online_ratio`, `returns_rate`

**3. Data Preprocessing**
- Standardized numerical features using `StandardScaler`
- Prepared scaled feature matrix for K-Means clustering
- Applied PCA for 2D cluster visualization

**4. Cluster Selection**
- Elbow Method — to analyze inertia
- Silhouette Score — to evaluate cluster separation
- Final number of clusters: **k = 3**

**5. K-Means Clustering**
- Trained the final K-Means model
- Assigned each customer to a segment
- Visualized clusters using PCA
- Compared customer behavior across segments

**6. Segment Profiling**
- Segment size analysis
- Average income, spending score, purchase frequency, order value, loyalty years, online ratio, and returns rate
- Business interpretation of each segment

**7. Export for Power BI**
- `customer_segments.csv` — customer-level data with segment labels
- `segment_summary.csv` — segment-level summary for dashboard and business insights

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C9ED9?style=flat)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)

---

## 💡 Key Findings

- **3 customer segments** were identified using K-Means clustering
- **High-Value Loyalists** are the most profitable and loyal customer group
- **Bargain Hunters** are the largest segment, with high online activity and moderate spending
- **At-Risk Customers** show the weakest engagement, lowest spending score, and highest returns rate
- Silhouette Score showed that **k = 3** gives the best cluster separation
- Segment-level analysis helps create more targeted marketing and retention strategies

---

## 👥 Customer Segments

| Segment | Segment Name | Customer Count | Main Characteristics |
|---|---:|---:|---|
| 0 | High-Value Loyalists | 120 | High income, high spending, frequent purchases, strong loyalty |
| 1 | Bargain Hunters | 270 | Largest group, younger customers, lower income, high online activity |
| 2 | At-Risk Customers | 110 | Low spending, low purchase frequency, high returns rate |

---

## 📊 Segment Interpretation

### Segment 0 — High-Value Loyalists

This segment includes customers with the highest annual income, highest spending score, highest purchase frequency, high average order value, and strong loyalty.

These customers are the most valuable for the business because they already show strong purchasing behavior and long-term engagement.

**Recommended actions:**
- Loyalty rewards
- Premium offers
- Personalized product recommendations
- Early access to new products
- Retention-focused campaigns

---

### Segment 1 — Bargain Hunters

This is the largest customer segment. These customers have lower income, moderate spending behavior, and high online purchase activity.

They are likely to respond well to digital campaigns, discounts, bundles, and price-based offers.

**Recommended actions:**
- Discount campaigns
- Bundle offers
- Online promotions
- Email and social media campaigns
- Affordable product recommendations

---

### Segment 2 — At-Risk Customers

This segment has the lowest spending score, lower purchase frequency, lower online activity, and the highest returns rate.

These customers may require reactivation and customer experience improvement before stronger upselling campaigns.

**Recommended actions:**
- Reactivation campaigns
- Return reason analysis
- Customer satisfaction surveys
- Service improvement
- Personalized retention offers

---

## 📈 Power BI Dashboard

A Power BI dashboard was created to make the segmentation results easier to understand for business users.

The dashboard allows users to compare customer segments by:
- Customer count
- Annual income
- Spending score
- Purchase frequency
- Average order value
- Loyalty years
- Online purchase ratio
- Returns rate

The dashboard helps translate machine learning results into clear business insights.

---

## 📌 Business Value

This project shows how customer segmentation can support marketing and business decision-making.

The results can help a company:
- Identify high-value customers
- Create personalized marketing campaigns
- Improve customer retention
- Reduce churn risk
- Understand customer behavior
- Improve campaign targeting
- Support data-driven decisions

---

## 👥 Team

**Nazerke Zhumadilova** · [@nazhmdt](https://github.com/nazhmdt)  
**Inzhu Nurlan** · [@InzhuNurlan](https://github.com/InzhuNurlan)

---

## 🎓 Course

**AI in Marketing** — Astana IT University  
Instructor: **Muhammed Ali Ibrahim**
