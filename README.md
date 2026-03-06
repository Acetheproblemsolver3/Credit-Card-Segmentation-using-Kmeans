# Credit Card Customer Segmentation using K-Means Clustering

## Project Overview

Customer segmentation is an important analytical task for financial institutions. By grouping customers with similar credit card usage behavior, banks can design targeted marketing strategies, personalize financial products, and better understand spending patterns.

This project applies **K-Means clustering**, an unsupervised machine learning algorithm, to segment credit card customers based on their financial behavior and transaction patterns.

The goal is to identify meaningful customer groups that share similar credit usage characteristics.

---

## Dataset

The dataset used in this project contains **credit card usage behavior of customers over a six-month period**.

Dataset source:

https://www.kaggle.com/datasets/arjunbhasin2013/ccdata

Key features in the dataset include:

- BALANCE – Remaining balance on the credit card
- PURCHASES – Total purchase amount
- CASH_ADVANCE – Cash withdrawn using the credit card
- CREDIT_LIMIT – Maximum credit limit
- PAYMENTS – Total payments made
- PURCHASE_FREQUENCY – Frequency of purchases
- CASH_ADVANCE_FREQUENCY – Frequency of cash withdrawals

These variables describe how customers interact with their credit cards.

---

## Methodology

The analysis followed these steps:

### 1. Data Preprocessing

- Missing values were handled
- Unnecessary identifiers were removed
- Features were scaled using **StandardScaler**

Feature scaling is important because **K-Means relies on distance calculations**, which can be affected if variables are on different scales.

---

### 2. Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand:

- distribution of financial variables
- customer spending patterns
- credit usage behavior

Visualization libraries such as **Matplotlib** and **Seaborn** were used.

---

### 3. Determining Optimal Number of Clusters

The **Elbow Method** was used to determine the optimal number of clusters.

Inertia values were calculated for cluster values ranging from **1 to 10**, and the elbow point was used to determine the most appropriate number of clusters.

---

### 4. Customer Segmentation using K-Means

After scaling the dataset, the **K-Means algorithm** was applied to segment customers.

The analysis resulted in **6 distinct customer clusters**, representing groups of customers with similar financial behavior.

---

## Results

The clustering algorithm identified **six customer segments** based on credit card usage patterns.

Examples of potential cluster characteristics include:

**Cluster 1 — High Value Customers**

- High credit limits
- Frequent purchases
- Higher spending levels

**Cluster 2 — Low Activity Customers**

- Low transaction frequency
- Low credit utilization
- Minimal spending

**Cluster 3 — Cash Advance Users**

- Frequent cash withdrawals
- Higher outstanding balances

These segments help organizations better understand how different customers interact with their credit products.

---

## Visualization

The clustering process includes visual analysis such as:

- Elbow Method plot (Inertia vs Number of Clusters)
- Cluster distribution visualizations

Example:

![Elbow Method](outputs/elbow_method.png)

---

## Business Applications

Customer segmentation can support several business decisions:

- Targeted marketing campaigns
- Customer retention strategies
- Credit limit adjustments
- Personalized financial products
- Customer risk monitoring

Financial institutions often use segmentation analytics to improve decision-making and customer experience.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Future Improvements

Potential improvements to this project include:

- Evaluating cluster quality using **Silhouette Score**
- Applying **PCA for improved cluster visualization**
- Comparing clustering algorithms such as **DBSCAN or Hierarchical Clustering**
- Creating detailed customer personas for each cluster

---

## How to Run the Project

1. Clone the repository

```bash
git clone https://github.com/Acetheproblemsolver3/Credit-Card-Segmentation-using-Kmeans
