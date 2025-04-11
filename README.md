🛍️ **Customer Behavior Clustering with Categorical Features**

This project explores customer behavior by applying clustering techniques on a dataset with categorical and numerical features. The analysis involves preprocessing, statistical testing, dimensionality reduction, and clustering to uncover hidden patterns in customer preferences.

📌 Objectives

- Cluster customers based on their behavior and attributes.
- Apply dimensionality reduction using PCA for visualization.
- Use statistical tests to explore feature relationships.

🔍 Features Used

The following features were selected for clustering:

- `Gender`
- `Item Purchased`
- `Location`
- `Shipping Type`
- `Payment Method`
- `Frequency of Purchases`
- `Subscription Status`
- `Age`
- `Purchase Amount (USD)`
- `Size` (ordinal: S, M, L, XL)

Encoding Strategy

- `Size` was encoded using `OrdinalEncoder` with custom order.
- All other categorical features were encoded using `OneHotEncoder`.

🧪 Statistical Analysis

The notebook includes several statistical tests to understand relationships between features:

- **Spearman Correlation** for detecting associations between ordinal/numerical features.
- **Chi-Square Test of Independence** to check dependence between categorical variables.
- **Cramér’s V** to measure the strength of association between categorical features.

These tests guide preprocessing and support interpretation of clustering results.

⚙️ Clustering Workflow

Dimensionality Reduction

- **PCA** was applied after encoding to reduce high-dimensional data.
- The number of components was selected based on the **explained variance ratio**.

Clustering Algorithms

- **KMeans Clustering** was used with the optimal number of clusters estimated using the **Elbow Method**.
- **Agglomerative Clustering** was also used to compare hierarchical clustering performance.

📊 Visualization

- **2D and 3D PCA scatter plots** were created using `plotly` to visualize clustering results.
- Plots help evaluate cluster separation and structure.

🎯 Marketing Strategy Implications

Cluster insights can support:

- Targeted marketing based on customer behavior.
- Improved segmentation for promotions or subscription offers.
- Data-driven decisions on product, shipping, and payment preferences.
