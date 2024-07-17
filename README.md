# CryptoClustering

This project uses Python and unsupervised learning to analyze cryptocurrency price changes.

## Steps

1. **Data Preparation**
    - Load `crypto_market_data.csv` into a DataFrame.
    - Normalize data using `StandardScaler`.
    - Create a scaled DataFrame with `coin_id` as the index.

2. **Elbow Method for Optimal k using Original Data**
    - Compute inertia for k values from 1 to 11.
    - Plot elbow curve to find the optimal k.

3. **K-means Clustering**
    - Cluster data using K-means with the best k.
    - Add cluster labels to the original DataFrame.
    - Scatter plot: `price_change_percentage_24h` vs `price_change_percentage_7d`.

4. **PCA Optimization**
    - Reduce to three principal components.
    - Create a PCA DataFrame with `coin_id` as the index.

5. **Elbow Method with PCA Data**
    - Compute inertia for k values from 1 to 11 on PCA data.
    - Plot elbow curve to find the optimal k.

6. **K-means Clustering with PCA**
    - Cluster PCA data using K-means with the best k.
    - Add cluster labels to the PCA DataFrame.
    - Scatter plot: `PC1` vs `PC2`.

## Tools

- Python
- Jupyter Notebook
- Pandas
- Scikit-learn
- hvPlot


## Contributors

- [Avinash K]([link to my GitHub profile](https://github.com/AVI-1213))
  
## Installation

```bash
pip install pandas scikit-learn hvplot

