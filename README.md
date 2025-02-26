# K-Means Clustering from Scratch
This repository contains a Python implementation of the K-Means clustering algorithm using NumPy and Pandas. The code demonstrates how to cluster data from the Iris dataset based solely on sepal measurements by iteratively assigning data points to clusters and updating centroids until convergence.

Overview
Data Loading:
The Iris dataset is loaded from a CSV file, and the 'Species' column is removed to focus on the numerical features (SepalLengthCm and SepalWidthCm).

Distance Calculation:
The Euclidean distance between points is computed using the built-in math.dist function.

Cluster Assignment:
Each data point is assigned to the nearest centroid using the update_cluster function.

Centroid Update:
The update_centroids function recalculates the centroids as the mean of the points in each cluster.

Iteration:
The algorithm iterates until either the centroids converge within a specified tolerance or the maximum number of iterations is reached.

Usage
Update Dataset Path:
Modify the file path in pd.read_csv() to point to your local copy of the Iris dataset.

Run the Script:
Execute the script using Python 3:

bash
Copy code
python kmeans.py

Output:
The console will display the centroid updates for each iteration and print the final centroids once convergence is reached.

Requirements
Python 3.x
NumPy
Pandas
Contributing
Contributions, suggestions, and bug fixes are welcome. Feel free to fork the repository and open a pull request with your improvements.
