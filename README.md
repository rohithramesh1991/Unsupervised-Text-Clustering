# Unsupervised-Text-Clustering
Step 1: Vectorization

TFIDF Vectorizer is used to create a vocabulary.
TFIDF is a product of how frequent a word is in a document multiplied by how unique a word is w.r.t the entire corpus.
ngram_range parameter : which will help to create one , two or more word vocabulary depending on the requirement.

Step 2: kmeans - Clustering
Grouping similar data points together and discover underlying patterns. 
To achieve this objective, K-means looks for a fixed number (k) of clusters in a dataset.
The K-means algorithm identifies k number of centroids, and then allocates every data point to the nearest cluster.
The ‘means’ in the K-means refers to averaging of the data; that is, finding the centroid.

Step 3 : Validation for the optimal number of clusters using ELBOW method:

The “elbow” method to help data scientists select the optimal number of clusters by fitting the model with a range of values for K. If the line chart resembles an arm, then the “elbow” (the point of inflection on the curve) is a good indication that the underlying model fits best at that point.
The total WSS(within-cluster sum of square) measures the compactness of the clustering and we want it to be as small as possible.
The Elbow method looks at the total WSS as a function of the number of clusters: One should choose a number of clusters so that adding another cluster doesn’t improve much better the total WSS.

How it calculates : 
* For each k, calculate the total within-cluster sum of square (wss).
* Plot the curve of wss according to the number of clusters k.
* The location of a bend (knee) in the plot is generally considered as an indicator of the appropriate number of clusters.
For detailed explanation kindly refer "https://medium.com/@rohithramesh1991/unsupervised-text-clustering-using-natural-language-processing-nlp-1a8bc18b048d"

## Note:
Please don't copy the code directly and try and execute as it will give you unresolved issue. You can use these funtion on your data, so the X_train comes from your data.
