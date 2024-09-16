# CryptoClustering


Determine the Optimal Value for \( k \) Using PCA Data

Apply the elbow method to the PCA data to find the best value for \( k \) by following these steps:

1. Generate a list of \( k \) values ranging from 1 to 11.
2. Create an empty list to hold the inertia values.
3. Use a for loop to compute the inertia for each \( k \) value.
4. Compile a dictionary with the data needed to plot the Elbow curve.
5. Create a line chart displaying the computed inertia values for each \( k \) to visually determine the optimal \( k \).

In your notebook, address the following questions: What is the best \( k \) value when using the PCA data? How does this compare to the best \( k \) value identified with the original data?

Cluster Cryptocurrencies with K-means Using the PCA Data

Follow these steps to cluster the cryptocurrencies based on the optimal \( k \) value from the PCA data:



1. Initialize the K-means model with the optimal \( k \) value.
2. Fit the K-means model to the PCA data.
3. Predict the clusters for the cryptocurrencies using the PCA data.
4. Create a copy of the DataFrame containing the PCA data and add a new column for the predicted clusters.
5. Generate a scatter plot using hvPlot with the following settings:
   - Set the x-axis to "price_change_percentage_24h" and the y-axis to "price_change_percentage_7d".
   - Color the points according to the K-means cluster labels.
   - Include the "coin_id" column in the `hover_cols` parameter to display the cryptocurrency name for each data point.

In your analysis, address the following question: How does using fewer features impact the clustering results with K-means?

Conclusion :

The project examines how reducing the number of features affects clustering with K-means. By comparing the clustering results from the original data with those from the PCA data, it aims to reveal the impact of dimensionality reduction on the clustering process.