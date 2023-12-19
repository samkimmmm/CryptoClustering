# CryptoClustering - Module 19 Challenge

# Overview
This challenge involved employing unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

# Technologies
* Pandas
* SciKit Learn

# Prepare the Data
A DataFrame with "coin_id" set as the index was created, utilizing "StandardScaler()" and "scikit-learn" to normalize the data in the CSV file.
<img width="1523" alt="Screenshot 2023-12-19 at 3 05 38 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/9a5204e2-3e0c-4314-bcb0-b624798dc5fa">

## Elbow Method for K Determination
### The best value for K was determined using the elbow method. An empty list stored the inertia values, and the results were plotted on an hvplot.
<img width="1266" alt="Screenshot 2023-12-19 at 3 06 51 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/cdc46970-dd1a-481f-b98b-4a2926048c9c">
What is the best value for K? 4

## Cryptocurrency Clustering
Clusters were predicted to group cryptocurrencies, and the results were plotted on a scatter plot with "PC1" on the x-axis and "PC2" on the y-axis.
<img width="1232" alt="Screenshot 2023-12-19 at 3 09 40 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/82a1d807-6b21-4ce0-8e91-b61d3cb8ee2b">

## A Principal Component Analysis (PCA) was performed to reduce the features to 3 principal components.
### What is the total explained variance of the three principal components? 89.50

## The elbow method on PCA data was used to find the best value for K.
<img width="1264" alt="Screenshot 2023-12-19 at 3 12 45 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/8a0fbe99-9d5f-497d-a999-33f791474852">
What is the best value for K when using the PCA data? 4
Does it differ from the best K value found using the original data? No

### Comparison of Clusters
Clusters created using PCA data were compared to the original scaled dataset.
<img width="1151" alt="Screenshot 2023-12-19 at 3 18 06 PM" src="https://github.com/samkimmmm/CryptoClustering/assets/135805393/d56070f0-9bea-4b69-85a3-8e362f8b986d">

# Analysis
#### After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?

  * **Answer:** Although the Elbow Data shows that the optimal value for k remains at 4, the clusters for each individual dataset proves to minimize the scatter of clusters.
