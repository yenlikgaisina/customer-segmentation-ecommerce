# Customer Segmentation for E-Commerce Churn Prevention

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3-orange?logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)

**Problem:** A transnational e-commerce business cannot tell which customers are drifting toward churn — or how to target win-back and retention campaigns effectively.

**Headline result:** K-Means clustering on RFM+ features identifies distinct customer segments from 541,909 UCI Online Retail transactions, enabling targeted retention and win-back strategies for high-value and lapsed groups.

---

## How to Run

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook notebook/customer_segmentation_ecommerce.ipynb
```

---

## Overview

This project applies unsupervised machine learning to segment e-commerce customers based on behavioural features derived from transactional data. Using the UCI Online Retail dataset, RFM-style features (Recency, Frequency, Monetary Value, Average Unit Price, Basket Size) are engineered at the customer level, then K-Means clustering identifies natural customer groupings. The segmentation enables targeted marketing: loyalty programmes for high-value customers, win-back campaigns for lapsed ones, and personalised promotions for growth-potential segments.

---

## Dataset

| Property | Detail |
|---|---|
| Source | UCI Machine Learning Repository — Online Retail |
| Records | ~541,909 transaction line items |
| Coverage | UK-based online retailer with international customers |
| Period | December 2010 — December 2011 |
| Access | Free download, no registration required |

---

## Engineered Features

| Feature | Description |
|---|---|
| Recency | Days since the customer's most recent purchase |
| Frequency | Total number of unique orders placed |
| Monetary (CLV) | Total revenue generated across all orders |
| Avg Unit Price | Mean price of items purchased |
| Basket Size | Mean items per order |

---

## Methods

| Stage | Technique | Purpose |
|---|---|---|
| Data cleaning | Remove cancellations, nulls, duplicates | Quality assurance |
| Feature engineering | RFM+ aggregation to customer level | Behavioural features |
| Cluster selection | Elbow Method, Silhouette Score, Dendrogram | Optimal k determination |
| Clustering | K-Means (k-means++, multiple inits) | Customer segmentation |
| Visualisation | PCA, t-SNE | 2D cluster validation |
| Profiling | Median feature comparison by cluster | Business interpretation |

---

## Key Findings

All specific metrics (cluster sizes, silhouette scores, PCA variance, segment profiles) are computed from the real UCI dataset and reported in the notebook.

---

## Repository Structure

```
customer-segmentation-ecommerce/
├── notebook/
│   └── customer_segmentation_ecommerce.ipynb
└── README.md
```

---

## Skills Demonstrated

Python · Pandas · NumPy · Scikit-learn · Matplotlib · Seaborn · K-Means · Hierarchical Clustering · PCA · t-SNE · RFM Analysis · Feature Engineering · Customer Segmentation · Unsupervised Learning

---

## Author

**Yenlik Gaisina** | Data and Analytics Consultant
[LinkedIn](https://linkedin.com/in/yenlik-gaisina) · [Portfolio](https://gaisina.co.uk)
