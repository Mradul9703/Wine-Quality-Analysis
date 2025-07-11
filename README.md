# Wine Quality Clustering

This project applies unsupervised machine learning to cluster **white wines** based on their physicochemical properties using the **K-Means** algorithm.

## Dataset

The dataset includes the following features:

| Fixed acidity        | Volatile acidity      | Citric acid           |
|----------------------|-----------------------|------------------------|
| Residual sugar       | Chlorides             | Free sulfur dioxide   |
| Total sulfur dioxide | Density               | pH                    |
| Sulphates            | Alcohol               | Quality (reference)   |

## Objective

To group white wines into clusters based on their chemical properties without using the quality label, and to evaluate the clustering performance using unsupervised learning techniques.

## Preprocessing

- The `quality` column was removed from the features.
- Features were scaled using **StandardScaler** to ensure equal contribution of all variables.

## Clustering Method

- **K-Means Clustering** was used to group the wines.
- The **Elbow Method** was applied to determine the optimal number of clusters.
- **Silhouette Score** was used to assess the clustering quality.

## Evaluation

- The silhouette score was used as a metric to determine how well-separated the clusters are.
- If the score is low or negative, it may indicate poor clustering performance or overlapping clusters.

## Technologies Used

- **Programming Language**: Python
- **Environment**: Google Colab
- **Libraries**:
  - `pandas`, `numpy` for data manipulation
  - `matplotlib`, `seaborn` for data visualization
  - `scikit-learn` for preprocessing, clustering, and evaluation

