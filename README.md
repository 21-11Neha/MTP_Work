# MTP_Work
I will be uploading my implementations here.
Dataset Link: https://archive.ics.uci.edu/ml/datasets/UrbanGB%2C+urban+road+accidents+coordinates+labelled+by+the+urban+center
# K means clustering 
Implemented using sklearn k means library
<br/>1: Select K points as initial centroids.
<br/>2: repeat
<br/>3: Form K clusters by assigning each point to its closest centroid.
<br/>4: Recompute the centroid of each cluster.
<br/>5: until Centroids do not change.

# spectral clustering
Implemented using sklearn spectral clustering library
Input: Similarity matrix S ∈ Rn×n, number k of
clusters to construct.
<br/>• Construct a similarity graph by one of the
ways described in Sect. 2. Let W be its
weighted adjacency matrix.
<br/>• Compute the unnormalized Laplacian L.
<br/>• Compute the first k eigenvectors u1,...,uk
of L.
<br/>• Let U ∈ Rn×k be the matrix containing the
vectors u1,...,uk as columns.
<br/>• For i = 1,...,n, let yi ∈ Rk be the vector corresponding to the i-th row of U.
<br/>• Cluster the points (yi)i=1,...,n in Rk with the
k-means algorithm into clusters C1,...,Ck.
Output: Clusters A1,...,Ak with
Ai = {j |yj ∈ Ci}
# 2-way spectral clustering
<br/>1: Input: A graph G = (V,E); its Laplacian matrix L; and r, a
threshold value
<br/>2: Find the second eigenvalue k2 of L and its associated
eigenvector x(2) 
<br/>3:  if
xi>=0 then vi is in C1, otherwise, vi is in C2;
<br/>4: Output: The resulting partition
# k-way spectral clustering
<br/>1: Input: A graph G = (V,E); and the number of desired
clusters, k
<br/>2: Find the first k eigenvectors of L and sort them in the
columns of matrix U. The i-th row of the matrix U will
represent node vi from graph G
<br/>3: Apply the k-means algorithm to the matrix U and find a k way partition 
<br/>5: Output: The final partition
