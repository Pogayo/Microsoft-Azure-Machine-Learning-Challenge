**Lesson 4:Supervised and unsupervised learning**

# Chapter 24- Clustering

>As the name suggests, clustering is the problem of organizing entities from the input data into a finite number of subsets or clusters; the goal is to maximize both intra-cluster similarity and inter-cluster differences.

##Applications of Clustering
- Personalization and target marketing
- Document classification- Tag documents into different tags which then can be used during searches for documents
- Fraud detection
- Medical imaging - eg differentiate between tissues
- City planning- Identify different types of houses

## Types of Clustering
- Centroid based clustering - based on distance of members from centroid of a cluster eg Kmeans
- Density based clustering - clusters members that are closely packed together. It can learn structures of arbitrary shapes
- Distribution based clustering - underlying assumption is that the data has an inherent disribution type- eg normal. The algorithm then clusters based on the probability of a member belonging to a certain distribution
- Hierachical clustering- The algorithm builds a tree of clusters.Best suited for hierachical data such as taxonomy.

## K-means clustering
- Centroid based unsupervised clustering algorithm.
- It creates up to a target(K) number of clusters and groups similar members together.
- Objective is to minimize intra-cluster distance

###Steps in K-means clustering
1. Initialize the centroids- Typically, the centroids will be randomly initialized
2. Cluster Assignment -based on euclidian distance from the centroid to the closest centroid
3. Move centroids
4. Check foe convergence. Two convergence criteria
    * A fixed number of iterations
    * Check how muc centroid location has changed as a result of new cluster membership. If total change is less than a given tolerance, it will assume convergence and stop. If criteria not met, iterate to step number 2.

### K-means module configurations in Azure ML
- **Number of centroids**- Algorithm starts with this number of clusters, not guaranteed to produce it in the end
- **Initialization approach**- to select the initial centroids. Options are
    * Random
    * First n
    * K-means ++
- **Distance metric** -default is Euclidian
- **Normalize features**
- **Assign label mode**- used when your dataset has the label column. Uses
    * Guide the selection of clusters
    * Fill in missing values
    * Can also ask the model to fill in the missing values in this column by using the label of the nearest member in the cluster
- **Number of iterations** - to check convergence

