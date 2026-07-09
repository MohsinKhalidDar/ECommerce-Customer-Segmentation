# ECommerce-Customer-Segmentation

Ecommerce Customer Segmentation is a machine learning notebook project that groups customers based on demographics, purchase behavior, web activity, and campaign response data. The goal is to identify useful customer segments that can support personalized marketing, retention planning, and promotional strategy.

## Dataset

The project uses `data/customers.csv`.

- 2,240 customer records
- 22 original features
- Demographic fields such as birth year, education, marital status, income, and children at home
- Purchase behavior across wines, fruits, meat, fish, sweets, and gold products
- Channel activity from web, catalog, and store purchases
- Campaign response and complaint indicators

## Workflow

```text
Data Cleaning
  -> Missing Value Handling
  -> Feature Engineering
  -> Outlier Removal
  -> Exploratory Data Analysis
  -> One-Hot Encoding
  -> Feature Scaling
  -> PCA Visualization
  -> Cluster Selection
  -> KMeans and Agglomerative Clustering
  -> Customer Segment Analysis
```

## Feature Engineering

The notebook creates several additional features:

- `Age`
- `Customer_Tenure_Days`
- `Total_Spending`
- `Total_Children`
- simplified `Education` groups
- `Living_With`

It also removes high-impact outliers, including customers with unrealistic ages and the extreme income value.

## Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Kneed
- Threadpoolctl

## Project Structure

```text
SmartCart-Customer-Segmentation/
|-- data/
|   `-- customers.csv
|-- images/
|   |-- agglomerative_clusters_3d.png
|   |-- cluster_count_distribution.png
|   |-- correlation_heatmap.png
|   |-- elbow_method_wcss.png
|   |-- elbow_vs_silhouette_score.png
|   |-- feature_pairplot_outlier_check.png
|   |-- income_vs_total_spending_by_cluster.png
|   |-- kmeans_clusters_3d.png
|   `-- pca_3d_projection.png
|-- notebooks/
|   `-- Smartcart_.ipynb
`-- README.md
```

## Results

The model identified **four customer segments**:

- Premium Customers
- Family Shoppers
- Budget Customers
- High ROI Customers
