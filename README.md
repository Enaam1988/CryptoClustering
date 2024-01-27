# CryptoClustering

## Introduction
This project aims to predict whether cryptocurrencies are affected by 24-hour or 7-day price changes using Python and unsupervised learning techniques.
## Instructions
1. **Load Data:**
   - Load `crypto_market_data.csv` into a DataFrame.

2. **Data Exploration:**
   - Get summary statistics and plot the data to understand its distribution.

3. **Data Preparation:**
   - Use `StandardScaler()` from scikit-learn to normalize the data.
   - Create a DataFrame with scaled data, setting "coin_id" as the index.

4. **Find Best Value for k (Original Scaled DataFrame):**
   - Use the elbow method to find the best value for k.
   - Plot a line chart to identify the optimal value for k.
   - Answer the question: What is the best value for k?

5. **Cluster Cryptocurrencies with K-means (Original Scaled Data):**
   - Initialize K-means model with the best k.
   - Fit and predict clusters on the original scaled DataFrame.
   - Create a scatter plot using hvPlot with PC1 and PC2.
   - Answer the question: What is the impact of using K-Means on the original scaled data?

6. **PCA and Explained Variance:**
   - Perform PCA on the original scaled DataFrame.
   - Retrieve explained variance for three principal components.
   - Answer the question: What is the total explained variance of the three principal components?

7. **Find Best Value for k (PCA Data):**
   - Use the elbow method to find the best value for k using PCA data.
   - Plot a line chart to identify the optimal value for k.
   - Answer the question: What is the best value for k when using PCA data? Does it differ from the original data?

8. **Cluster Cryptocurrencies with K-means (PCA Data):**
   - Initialize K-means model with the best k.
   - Fit and predict clusters on the PCA data.
   - Create a scatter plot using hvPlot with price_change_percentage_24h and price_change_percentage_7d.
   - Answer the question: What is the impact of using fewer features to cluster the data using K-Means?

## Rewind
If you need a refresher on creating composite plots, refer to the relevant module or check the [hvPlot documentation on Composing Plots](<provide link here>).
