# Crypto-Clustering-Unsupervised-Machine-Learning
## This analysis uses Python and unsupervised machine learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.
### Jupyter Notebook file "Crypto_Clustering.ipynb" takes in file "Resources/crypto_market_data.csv" containing crypocurrency information and performs a sequence of steps.
Using the original file data:
1. Use the `StandardScaler()` module from scikit-learn to normalize the data from the CSV file.
2. Use the elbow method to determine the best value for k.
3. Cluster the cryptocurrencies with k-means and plot the results.
Optimize Clusters with Principal Component Analysis:
1. Create a PCA model and calculate the explained variance to determine a sufficient total explained variance.
2. Use the elbow method for the PCA data to determine the best value for k.
3. Cluster the PCA data with k-means and plot the results.

After visually analyzing the cluster analysis results, there is an impact of using fewer features to cluster the data using K-Means. The elbow curves are very similar, but using fewer features yields a similar result with a much cleaner scatter plot with clusters that are easier to identify.
![comparison_charts.jpg](/Resources/comparison_charts.jpg "Comparison of both clustering methods")