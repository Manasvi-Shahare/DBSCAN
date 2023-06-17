# DBSCAN
Data Mining Techniques - DBSCAN Algorithm on Breast Cancer Dataset

This project aims to analyze the Breast Cancer Wisconsin Diagnos- tic Dataset using supervised and unsupervised machine learning methods. The dataset contains information about breast cancer tumors, including numerical features that describe each tumor. We are trying to solve two problem definitions. The first problem definition is to classify each tumor as either malignant or benign based on its numerical features. The second problem definition is to cluster the tumors into groups based on their similarity. For the classification problem, methods such as Multi-Layer Perceptron, K-Nearest Neighbor, and Random Forest Classifier will be employed. These algorithms will be evaluated using metrics such as accuracy, precision, recall, and F1-score. For the clustering problem, unsupervised learning methods such as DBSCAN clustering and Spectral Clustering will be used to group similar tumors together based on their features. The performance of each clustering algorithm will be evaluated using metrics such as the Silhouette Coefficient scores and the Normalized Mutual Information scores.


I implemented the DBSCAN algorithm. 

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) is a popular clustering algorithm used in ma- chine learning and data mining. It is an unsupervised ma- chine learning algorithm which is designed to identify clus- ters of data points in a dataset based on the density of the points. DBSCAN was developed to address the limitations of traditional clustering algorithms. DBSCAN is able to dis- cover clusters of arbitrary shape, making it more flexible and versatile than other clustering algorithms. Another key motivation for DBSCAN is its ability to handle noise and outliers.
For DBSCAN, the most important parameters that need to be set are epsilon and MinPts. The parameters must be specified by the user.
– MinPts : represents the minimum number of points re-
quired in that neighborhood for a data point to be consid-
ered part of a cluster.
– Eps: represents the radius of a neighborhood around each
data point.


The algorithm works as follows:
(1) Choose a random unvisited point in the dataset.
(2) Find all the neighbors of that point within eps distance.
(3) If the point has at least MinPts points within eps distance,
create a new cluster and add all neighbor points to it oth-
erwise label it as noise.
(4) Expand the cluster by recursively adding all points that
are within eps distance of any point already in the cluster.
(5) Choose a new, unvisited point and continue the process
until no more points can be added to the cluster.
(6) The algorithm terminates after all points have been visited.
