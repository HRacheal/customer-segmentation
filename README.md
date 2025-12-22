# Customer Segmentation using Unsupervised Machine Learning

## Overview
This project applies unsupervised machine learning techniques to segment mall customers into distinct groups based on their demographic and spending behavior. The goal is to help businesses better understand customer patterns and design targeted marketing strategies.

## Problem Statement
Businesses often struggle to personalize marketing efforts due to limited insight into customer behavior. Without segmentation, marketing campaigns can be inefficient and fail to address customer needs effectively.

## Objective
To identify meaningful customer segments using unsupervised learning techniques based on age, income, and spending behavior.

## Dataset
- **Source:** Mall_Customers.csv
- **Size:** 200 customers
- **Features:**
  - CustomerID: Unique identifier
  - Gender: Customer gender
  - Age: Customer age (18–70)
  - Annual Income (k$): Income range ($15k–$137k)
  - Spending Score (1–100): Mall-assigned spending behavior score

## Methodology
### 1. Data Preprocessing
- Checked for missing values (dataset was clean)
- Encoded categorical features (Gender) using one-hot encoding
- Scaled numerical features using StandardScaler

### 2. Exploratory Data Analysis (EDA)
- Analyzed feature distributions
- Visualized relationships using pair plots and scatter plots

### 3. Clustering Techniques
Two clustering algorithms were implemented and compared:
- **K-Means Clustering**
- **Hierarchical Clustering (Agglomerative – Ward linkage)**

### 4. Dimensionality Reduction & Visualization
- Principal Component Analysis (PCA)
- t-SNE for visual cluster separation

### 5. Evaluation
- Silhouette Score used to assess cluster quality

## Results & Key Findings
- Distinct customer segments were identified based on combinations of:
  - High vs low income
  - High vs low spending behavior
- These segments can be mapped to customer personas such as:
  - High-income high-spenders
  - Budget-conscious customers
  - Low-income low-spenders

### Model Performance
| Model | Silhouette Score |
|------|------------------|
| K-Means | 0.350 |
| Hierarchical (Ward) | 0.348 |

K-Means performed marginally better, producing slightly more compact and well-separated clusters.

## Business Value
- Enables targeted marketing strategies
- Improves customer engagement and satisfaction
- Supports data-driven decision-making in retail environments

## Technologies Used
- **Python**
- **Pandas, NumPy**
- **Scikit-learn** (KMeans, AgglomerativeClustering, StandardScaler)
- **Matplotlib, Seaborn**
- **SciPy** (Hierarchical clustering)

## Key Learnings
- Importance of feature scaling in clustering
- How silhouette score helps evaluate cluster quality
- Trade-offs between centroid-based and hierarchical clustering
- Visualization techniques improve interpretability of high-dimensional data


