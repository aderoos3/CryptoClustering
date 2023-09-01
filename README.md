# CryptoClustering

The goal of this assignment was to categorize cryptocurreny data using unsupervised learning. I started with the usual things to prepare. It was also given in the starter code. Import dependencies, get the csv file into a DataFrame, look at the summary stats, and look at the data in a plot. 

Next I needed to scale the data so they were all on the same measure. I don't know if measure is the right word, but they were all a similar scale. I made a new DataFrame with the scaled data and added the crypto names. I found the best k value by looping through a list using KMeans. This made it so I could make an elbow curve. This elbow curve looked a little unusual with a ledge between 4 and 5. The elbow curve starts to get fewer distinct points, and the last point is an option for the best k value. Using this k value I can make the hvplot scatter plot. I had to fit and predict with the DataFrame and then make a new DataFrame with the prediction information. Then I was able to graph it. 

Next I wanted to optimize the clusters with PCA. I used three clusters and made an array with the information and found the variance ratio. I needed to make another elbow curve to find the best k value in this instance. It was a similar process of looping through k values, but I found that 4 was the best k value this time. This time I used 4 clusters to fit and predict the PCA model and then graph it. 

I compared the two graphs with composite graphs. The two elbow curves and the two scatter plots. 
