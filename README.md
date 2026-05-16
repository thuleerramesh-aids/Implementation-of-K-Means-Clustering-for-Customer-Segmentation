# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

**Step 1:** Start the program.

**Step 2:** Read the customer dataset (`Mall_Customers.csv`).

**Step 3:** Select **Annual Income** and **Spending Score** columns.

**Step 4:** Apply **K-Means clustering** to divide customers into **5 clusters**.

**Step 5:** Plot the clusters and mark cluster centers on the graph.

**Step 6:** Display the graph and stop the program.


## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: THULEER R
RegisterNumber:212225230285

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans
data = pd.read_csv("Mall_Customers.csv")
X = data.iloc[:, [3, 4]].values
kmeans = KMeans(n_clusters=5, random_state=0)
y_kmeans = kmeans.fit_predict(X)
plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')
plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")
plt.show()
*/
```

## Output:
<img width="185" height="121" alt="image" src="https://github.com/user-attachments/assets/a7843288-6b6c-48e7-8466-a56a1a1b0c20" />
<img width="255" height="196" alt="image" src="https://github.com/user-attachments/assets/6cbf456c-91b0-460d-abe9-53af7d5747d3" />




## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
