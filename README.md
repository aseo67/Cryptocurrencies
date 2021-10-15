# Cryptocurrencies Analysis
Module 18 Challenge Files
- [crypto_clustering.ipynb](https://github.com/aseo67/Cryptocurrencies/blob/main/crypto_clustering.ipynb)
- [crypto_data.csv](https://github.com/aseo67/Cryptocurrencies/blob/main/crypto_data.csv)
- [Screenshots](https://github.com/aseo67/Cryptocurrencies/tree/main/Screenshots)


## Overview of Analysis
An investment bank company is interested in offering a new cryptocurrency investment portfolio for its customers. As they are new to the space, they are looking to undersand what cryptocurrencies are on the trading market, and how they might be grouped or classifed into a classification system. Given the output is unknown, this analysis utilizes unsupervised learning - specifically a clustering algorithm - to group the cryptocurrencies

## Results

### Data Preprocessing

Dataframe (crypto_names_df) created containing cryptocurrency names (CoinName)
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20crypto_names_df.png)

Dataframe (X) of data with text features converted to numerical variables
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20X.png)

Data standardized (X_scaled) using StandardScaler()
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20X_scaled.png)

### Reducing Data Dimensions with PCA

PCA used to reduce dimension to 3 principal components
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20PCA.png)

DataFrame (pcs_df) created with 3 principal components
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20pcs_df.png)

### Cryptocurrencies Clustered Using K-Means

Best value found for _k_ using Elbow Curve
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20Elbow%20Curve.png)

K-Means run with _k=4_
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20K-Means%20Predictions.png)

DataFrame (clustered_df) created with predicted clusters and cryprocurrencies' features
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20clustered_df.png)

### Visualizations of Cryptocurrencies' Results

3-D Scatter of Clusters.
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%203D-Scatter.png)

Table of tradable cryptocurrencies using hvplot.table
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20hvplot%20table.png)

Total Number of Tradable Cryptocurrencies
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20Total%20Number%20of%20Tradable.png)

DataFrame (plot_df) created for scatter plot, using scaled data (of 'TotalCoinSupply' and 'TotalCoinsMined')
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20plot_df.png)

Scatter plot using hvplot.scatter
![Screenshot](https://github.com/aseo67/Cryptocurrencies/blob/main/Screenshots/Screenshot%20hvplot%20scatter.png)
