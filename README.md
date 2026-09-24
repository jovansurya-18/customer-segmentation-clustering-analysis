# Customer Segmentation with Clustering

An unsupervised machine learning project exploring customer segmentation using clustering techniques on a real-world e-commerce dataset.

## Overview

Understanding customer behaviour is important for developing targeted marketing strategies, improving customer engagement, and allocating resources effectively.

This project uses unsupervised machine learning to identify distinct customer segments based on purchasing behaviour and demographic characteristics, without relying on predefined customer labels.

The analysis follows an end-to-end data science workflow, including data preprocessing, feature engineering, exploratory data analysis, clustering, cluster validation, and dimensionality reduction.

## Dataset

The dataset is a real-world, transnational e-commerce dataset containing customers from **five continents and 47 countries**.

The analysis focuses on customer characteristics and purchasing behaviour, with engineered features used to better capture differences between customers.

## Methodology

### 1. Data Cleaning and Preprocessing

The dataset was prepared for analysis by:

* Handling missing values
* Correcting data types
* Removing duplicate records
* Preparing the data for feature engineering and clustering

### 2. Feature Engineering

Five additional features were engineered to better capture customer behaviour and characteristics.

These features were stored in a separate dataframe specifically prepared for the clustering analysis.

### 3. Exploratory Data Analysis

Exploratory data analysis was performed on both the original and feature-engineered datasets to examine:

* Feature distributions
* Customer behaviour
* Relationships between variables
* Potential differences between customer groups

### 4. K-Means Clustering

K-Means clustering was used to group customers into segments without predefined labels.

To determine the appropriate number of clusters, three complementary approaches were considered:

* Elbow Method
* Silhouette Analysis
* Agglomerative Hierarchical Clustering using a dendrogram

The analysis selected **5 clusters** as the final solution.

### 5. Dimensionality Reduction

Two dimensionality reduction techniques were used to visualise the clustering results:

* Principal Component Analysis (PCA)
* t-Distributed Stochastic Neighbor Embedding (t-SNE)

PCA provided a 2D representation of the clusters, while t-SNE produced a clearer visual separation between the five groups.

## Results

The analysis identified **five customer segments** with differences primarily related to **recency and age**.

Other characteristics, including customer lifetime value (CLV) and average unit cost, remained relatively consistent across the clusters.

The segments showed nuanced differences rather than completely distinct customer profiles, reflecting the complexity of real-world e-commerce behaviour.

### Customer Segments

| Cluster   | Key characteristics                                                                           |
| --------- | --------------------------------------------------------------------------------------------- |
| Cluster 0 | Moderately active customers with slightly higher purchase frequency and marginally higher CLV |
| Cluster 1 | Higher purchase recency and slightly higher average unit cost                                 |
| Cluster 2 | Older customers with behavioural characteristics broadly similar to the overall dataset       |
| Cluster 3 | Youngest customer segment, with purchasing behaviour broadly aligned with the other groups    |
| Cluster 4 | Very high recency, indicating lower recent engagement, with an older customer profile         |

## Visualisation

PCA provided a rough two-dimensional representation of the customer segments but showed limited separation.

t-SNE produced a clearer visualisation, with the five clusters distinctly separated in two-dimensional space. This suggests that the underlying customer behaviour contains non-linear structure that is not fully captured by PCA.

## Key Takeaways

* Unsupervised learning can be used to identify customer segments without predefined labels.
* **Recency and age** were the most influential characteristics differentiating the customer segments.
* CLV and average unit cost were relatively stable across the clusters.
* Combining multiple cluster-validation techniques helped inform the selection of **five clusters**.
* t-SNE provided clearer visual separation than PCA for this dataset.
* The resulting segmentation can provide a foundation for more targeted marketing and customer engagement strategies.

## Technologies & Techniques

* Python
* Pandas
* NumPy
* Scikit-learn
* K-Means Clustering
* Agglomerative Hierarchical Clustering
* PCA
* t-SNE
* Exploratory Data Analysis

## Project Structure

```text
customer-segmentation-clustering-analysis/
│
├── README.md
├── customer_segmentation_clustering_analysis.ipynb
└── customer_segmentation_clustering_analysis_report.pdf
```

## Author

**Jovan Surya**

Data Science, Machine Learning & AI
