# CryptoClustering

This challenge used unsupervised learning to predict if cryptocurrencies are affected by 24-hr or 7-day price changes.

To achieve this the data first needed to be prepared with StandardScaler() from scikit-learn into a new DataFrame that still used the coin_id index from the original DataFrame.

The elbow method was applied to the original scaled data to find the best value of K. 
  - The result was 4.

With a k of 4, the k-means model was performed, clusters were predicted, a new DataFrame formed, and Scatterplot was created to compare the clusters. The cryptocurrency of the data was added to the hover of the plot. 

Principal Component Analysis was then implemented to reduce the features down to three principal components. 
The total variance of the PCs was 89.5%.

The elbow method was applied to the PCA data to find the best value of K. 
  - The result was also 4.

With a k of 4, the k-means model was performed, clusters were predicted, a new DataFrame formed, and Scatterplot was created to compare the clusters. The cryptocurrency of the data was added to the hover of the plot. 

Lastly, the elbow plots and the scatterplots were composited to easily compare the original scaled data with the three-feature PCA data. 


###### Cited Sources: Bootcamp Spot in-class assignments
