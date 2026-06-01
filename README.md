# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import libraries and load the customer dataset.
2. Select important customer features for clustering.
3. Train the KMeans model with required clusters.
4. Group customers into segments and visualize the clusters. 

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: Farzana M
RegisterNumber:  212225040087
*/
```
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
# Simple K-Means Clustering Program for Customer Segmentation

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

data = pd.read_csv("Mall_Customer.csv")

X = data.iloc[:, [3, 4]].values

kmeans = KMeans(n_clusters=5, random_state=0)

y_kmeans = kmeans.fit_predict(X)

plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)

# Plot centroids
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')

# Labels
plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")

plt.show()
```

## Output:
<img width="1535" height="809" alt="Screenshot 2026-06-01 113853" src="https://github.com/user-attachments/assets/7a8059ee-fac3-4bad-91f7-66a72b9a89d8" />




## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
