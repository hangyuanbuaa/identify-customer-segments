# Readme

This is my work for Udacity Data Scientist Nanodegree project about Unsupervised Learning. The purpose of this project is to identify segments of the population that form the core customer base for a mail-order sales company in Germany. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns.

The data is provided by Bertelsmann Arvator Analytics, and represents a real-life data science task.
My approach is to clean up the messy data first, in order to prepare a suitable dataset for general machine learning algorithms. Afterwards, apply feature transformation, including feature scaling and Principal Component Analysis, to the dataset, which allows for clustering the general population and already existing customer data using the K-Means.

Then the key is to compare the cluster distribution of demographics data with customer data. Mismatches, such as the proportion of persons in a cluster being higher/lower in the customer data than the general population suggest it to be a target/not a target.  

To interpret the results, apply `inverse_transform()` method of the PCA and scaler objects to transform centroids back to the original space, and use the most important features of the centroids to represent the cluster.
