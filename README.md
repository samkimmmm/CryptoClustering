# CryptoClustering - Module 19 Challenge

# Overview
This challenge required the use of unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

# Technologies
* Pandas
* SciKit Learn

# Prepare the Data
A Dataframe with the "coin_id" set as the index was created once the "StandardScaler()" and "scikit-learn" was used to normalize the data in the CSV file.
<img width="1523" alt="Screenshot 2023-12-19 at 3 05 38 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/9a5204e2-3e0c-4314-bcb0-b624798dc5fa">

## Utilizing the elbow method, the best value for K was found by creating an empty list to store the inertia values. The results were then plotted on an hvplot.
<img width="1266" alt="Screenshot 2023-12-19 at 3 06 51 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/cdc46970-dd1a-481f-b98b-4a2926048c9c">
What is the best value for K? 4

## Clusters were then predicted to cluster the cryptocurrencies into groups. The results were then plotted on a scatter plot with the x-axis set to "PC1" and the y-axis set to "PC2".
<img width="1232" alt="Screenshot 2023-12-19 at 3 09 40 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/82a1d807-6b21-4ce0-8e91-b61d3cb8ee2b">

## A Principal Component Analysis (PCA) was performed to reduce the features to 3 principal components.
### What is the total explained variance of the three principal components? 89.50

## Using the elbow method on the PCA data, the best value for K was found.
<img width="1264" alt="Screenshot 2023-12-19 at 3 12 45 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/8a0fbe99-9d5f-497d-a999-33f791474852">
What is the best value for K when using the PCA data?
Does it differ from the best K value found using the original data?

## Clusters were created using the PCA data, then compared to the original scaled dataset.
<img width="1151" alt="Screenshot 2023-12-19 at 3 18 06 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/d56070f0-9bea-4b69-85a3-8e362f8b986d">

# Analysis
#### After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?

  * **Answer:** Although the Elbow Data shows that the optimal value for k remains at 4, the clusters for each individual dataset proves to minimize the scatter of clusters

