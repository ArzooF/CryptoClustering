# CryptoClustering

## Repository Setup

-- Created a new repository named CryptoClustering for this project. 
-- Cloned and perfomred initial push.
-- Cloned the newly created repository to the computer and pushed all changes to GitHub.

## Files and Preparation

-- Downloaded the files from the provided module link.
-- Renamed Crypto_Clustering_starter_code.ipynb to Crypto_Clustering.ipynb.

## Data Loading

-- Loaded the crypto_market_data.csv file into a DataFrame.
-- Obtained the summary statistics and plot the data to understand its structure before processing.

## Data Normalization

-- Used StandardScaler from scikit-learn to normalize the data.
-- Created a DataFrame with the scaled data, setting the "coin_id" from the original DataFrame as the index.

## Elbow Method for k-value

-- Created a list of k-values from 1 to 11 and an empty list to store inertia values.
-- Used a for loop to compute the inertia for each k-value, stored the results in a dictionary, and ploted an elbow curve to determine the best k-value.

## Clustering with K-Means (Original Data)

-- Initialized and fit the K-Means model with the best k-value determined from the elbow method.
-- Predicted clusters and added a new column with the predicted clusters to the original data.
-- Created a scatter plot using hvPlot with specified axes and hover columns.

## Principal Component Analysis (PCA)

-- Performed PCA on the scaled data to reduce it to three principal components.
-- Retrieved the explained variance and calculated the total explained variance of the three components.
-- Created a new DataFrame with the PCA data, setting the "coin_id" as the index.

## Elbow Method for PCA Data

-- Repeated the elbow method steps using the PCA data to determine the best k-value.
-- Plotted the elbow curve and compared the best k-value with the original data.

## Clustering with K-Means (PCA Data)

-- Initialized and fit the K-Means model with the best k-value for PCA data.
-- Predicted clusters and added them to the PCA DataFrame.
-- Created a scatter plot using hvPlot to visualize the PCA clusters and analyzed the impact of using fewer features.