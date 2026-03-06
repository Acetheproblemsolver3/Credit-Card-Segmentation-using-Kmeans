# Credit Card Customer Segmentation using K-Means Clustering

## Project Overview

Customer segmentation is an important analytics task for financial institutions. By grouping customers with similar credit card usage behavior, banks can design targeted marketing strategies, adjust credit limits, and better understand spending patterns.

This project applies **unsupervised learning using the K-Means clustering algorithm** to segment credit card customers based on their financial behavior and transaction patterns.

The goal is to identify distinct customer groups that share similar credit usage characteristics.

---

## Dataset

The dataset used for this project comes from Kaggle.

It summarizes the **usage behavior of approximately 9000 active credit card holders over a period of six months**, with multiple behavioral variables describing spending and account activity. :contentReference[oaicite:0]{index=0}

Dataset link:  
https://www.kaggle.com/datasets/arjunbhasin2013/ccdata

Examples of features in the dataset include:

- Balance
- Purchases
- Cash Advance
- Credit Limit
- Payments
- Minimum Payments
- Purchase Frequency
- Cash Advance Frequency

These variables represent how customers use their credit cards.

---

## Methodology

The following steps were performed during the analysis:

### 1. Data Preprocessing

- Removed unnecessary identifiers
- Handled missing values
- Normalized features to ensure equal scaling

Scaling is important because **K-Means relies on Euclidean distance**, making it sensitive to differences in feature magnitude. :contentReference[oaicite:1]{index=1}

---

### 2. Exploratory Data Analysis

Initial analysis was conducted to understand:

- spending patterns
- credit usage behavior
- distribution of financial features

---

### 3. Determining the Optimal Number of Clusters

The **Elbow Method** was used to determine the appropriate number of clusters for K-Means.

The elbow point indicates where adding more clusters does not significantly improve clustering performance.

---

### 4. Customer Segmentation using K-Means

The K-Means clustering algorithm was applied to group customers into segments based on behavioral similarity.

Customers with similar spending and credit usage characteristics are grouped together.

---

## Results

The clustering algorithm successfully identified distinct customer segments with different credit usage patterns.

Example cluster characteristics include:

**Cluster 1 – High Value Customers**

- High credit limits
- High purchase frequency
- High transaction amounts

**Cluster 2 – Low Activity Customers**

- Low credit utilization
- Few transactions
- Minimal spending

**Cluster 3 – Cash Advance Users**

- Frequent cash withdrawals
- Higher balances
- Moderate purchase activity

These segments can help financial institutions understand customer behavior and tailor services accordingly.

---

## Visualization

The clustering results were visualized using dimensionality reduction techniques to display customer groups in two-dimensional space.

Example visualizations include:

- Elbow Method plot
- Cluster scatter plots

---

## Business Applications

Credit card customer segmentation can support several business decisions:

- Targeted marketing campaigns
- Customer retention strategies
- Credit risk monitoring
- Personalized financial products
- Credit limit optimization

Banks commonly use segmentation analytics to better understand customer financial behavior.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Future Improvements

Potential improvements to this project include:

- Using **Silhouette Score** to evaluate clustering quality
- Testing other clustering algorithms (DBSCAN, Hierarchical Clustering)
- Applying **PCA for better cluster visualization**
- Building customer personas for each cluster

---

## How to Run the Project

1. Clone the repository

2. Install required dependencies

3. Open the notebook inside the notebooks folder and run the analysis.

---
