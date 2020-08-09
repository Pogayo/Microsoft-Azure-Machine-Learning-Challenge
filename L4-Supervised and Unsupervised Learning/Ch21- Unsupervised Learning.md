**Lesson 4:Supervised and unsupervised learning**

# Chapter 21- Unsupervised Learning

>In unsupervised learning, algorithms learn from unlabeled data by looking for hidden structures in the data.

- Obtaining unlabeled data is comparatively inexpensive
- unsupervised learning can be used to uncover very useful information in unlabeled data

##Types of unsupervised machine learning
###1. Clustering
Organizes entities from input data into finite number of subsets called clusters

###2. Feature Learning(Representation Learning)
Transforms sets of inputs into other inputs that are potentially more useful in solving a given problem.

###3. Anomaly detection
Identify two major groups- Normal and abnormal(anomalous)

**Examples**
K-means clustering, Auto-encoders, Principal component analysis(PCA)

# Chapter 22- Semi-supervised Learning
>Semi-supervised learning combines the supervised and unsupervised approaches; typically it involves having small amounts of labeled data and large amounts of unlabeled data.

##Approaches to semi-supervised learning
- Self-training- Train a model on the labeled data and use it to predict the labels of the unlabeled data resulting in a fully labeled dataset.
- Multi-view training- Train multiple models on various views of the data including feature selections, parts and model architecture
- Self-ensemble training- Similar to multi-view training except you use a single model with various hyperparameters


