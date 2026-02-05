## Customer Segmentation using K-Means Clustering
 # Project Overview

This project focuses on segmenting bank customers based on their behavioral and financial attributes using unsupervised machine learning (K-Means clustering).
The goal is to identify distinct customer groups, analyze their churn behavior, and derive actionable business insights to improve customer retention and value.

 # Objectives

1) Segment customers based on transaction behavior and credit usage

2) Identify high-risk churn customer groups

3) Validate customer segments using churn data

4) Provide data-driven business recommendations

 # Dataset

Source: BankChurners Dataset

Each row represents a unique customer

 # Features include:

1) Transaction behavior

2) Credit usage

3) Account engagement

4) Demographic attributes (used only for interpretation)

-  The churn label (Attrition_Flag) was excluded during clustering to avoid data leakage and later reintroduced for validation.

 # Tools & Technologies

1) Python

2) Pandas, NumPy

3) Scikit-learn

4) Matplotlib, Seaborn

5) Jupyter Notebook

 # Project Workflow

- Data Loading & Exploration

- Checked dataset structure, data types, missing and duplicate values

- Data Preprocessing

- Dropped churn labels before clustering

- Selected numeric behavioral and financial features

- Detected and capped outliers using the IQR method

- Standardized features using StandardScaler

- Clustering

- Applied K-Means clustering with k-means++ initialization

- Determined optimal number of clusters using:

- Elbow Method

- Silhouette Score

- Final number of clusters: 4

- Cluster Profiling

- Analyzed cluster-wise averages of numeric features

- Interpreted customer behavior patterns

- Used demographic features for post-cluster interpretation

- Churn Validation

- Reintroduced churn labels after clustering

- Compared churn rates across clusters to identify high-risk segments

 # Visualization

- Used PCA to project clusters into 2D space for visualization

- PCA was used strictly for visualization, not for model validation

 # Key Cluster Insights

- Cluster 0 – Credit-Dependent Loyal Customers
Low credit limit but high utilization with very low churn.

- Cluster 1 – Highly Active Core Customers
Highest transaction frequency and strong engagement.

- Cluster 2 – Premium Low-Risk Customers
Highest credit limits, low utilization, and moderate churn.

- Cluster 3 – High Churn Risk Customers
Low engagement, low utilization, and the highest churn rate.

 #  Business Recommendations

1) Target high-churn clusters with retention campaigns and personalized offers

2) Upsell premium services to highly active customers

3) Improve engagement strategies for low-utilization premium customers

4) Offer controlled credit optimization and financial tools to credit-dependent users

 # Limitations and Future Work

- Clustering performance depends on feature selection and scaling

- PCA was used only for visualization, not dimensionality reduction

- Future work could include DBSCAN or RFM-based customer segmentation

 #  Conclusion

This project demonstrates how unsupervised learning can be effectively used for customer segmentation, validated using churn behavior, and translated into practical business strategies.
The approach provides valuable insights for customer retention and engagement optimization.
