**Lesson 5: Applications of Machine Learning**

# Chapter 11- Similarity Learning
- Closely related to both classification and regression
- It uses a different type of objective function
- Often used in recommendation systems
- Often used in solving verification problems eg speech verification, face

## Similarity learning as a supervised learning approach
###as a classification problem
The similarity function maps pairs of entities to to a finite number of similarity levels(ranging from 0/1 to any number of levels)
### As a regression problem
The similarity function maps pairs of entities to numerical values.

**Ranking similarity learning** is a variation of this approach where the supervision is weakened from an exact measure to an ordering measure. The approach is better fit for real life large scale problems.

Deep learning algorithms are a special case of machine learning  algorithms that have the capability to learn complex, non-linear functions from data. 

## Recommender Systems
Are an application of similarity learning
Main aim is to recommend one or more items to users of a system

###Recommender systems approaches

Content based |   Collaborative filtering
---------|------------
Make use of properties for both items and users| uses only identifiers for users and items
User properties: age, gender, region| Gets information from a matrix of ratings
Item properties: manufacturer, author etc| Ratings can be explicit or implicit

Singular Value Decomposition algorithm - Collaborative filtering

# Chapter 15: Text Classification
Requires text to be in numerical format, a process known as **text embedding**

Text embedding has two forms
- Word embedding - can be used for complex scenarios such as Machine Translation
- Scoring -calculate a score for a word that is related to the importance of the word in the text

##  Text classification pipeline

- Text normalization- removing stop words, tokenization, spellcheck, stemming,lowercase 
- Feature extraction- identify vecabulary, vectorize (TF-IDF, word embeddings)
- Train a classification model

Note: use the same vocabulary as in the train set for the test set

# Chapter 17: Feature Learning
aka representation learning used to transfer set of inputs into new inputs

##Supervised approach
New features are learned using data that has already been labeled.

Suitable for:
- Datasets that have categorical features with high cardinality
- Image classification

##Unsupervised approach
Based on learning the new features without having labelled input data
Examples:
- Clustering
- Principal Component Analysis(PCA)
- Independent Component analysis
- Autoencoder(Deep learning)
- Matrix factorization

# Chapter 18: Applications of feature learning
1. Image classification
2. Image search
3. Feature embedding

##Image classification with Convolutional Neural Networks
1. Step 1: (Convolutional layer) Learn local patterns
2. Step 2: (Max-pooling layer) Downsample and make translation invariant
3. Step 3: (Dense layer) Densely connects all outputs to learn classification

## Image search with autoencoders
Used for unsupervised learning.
Trains to reproduce its own inputs.
Produces the feature vector.

##Anomaly Detection
**Anomaly detection** is a machine learning technique concerned with finding data points in a dataset that deviate significantly from the norm.

These anomalies can be of interest, since they may be the result of bad data, unusual behavior, or important exceptions to the typical trends.

Usually the number of abnormal entities is much less than th number of normal entities.
##Supervised anomaly detection
- Binary classification problem where entities are classified as normal or abnormal
- Highly imbalanced classes
- Labels available before
##Unsupervised anomaly detection
- A problem of identifying two major groups(clusters) of entities.
- Highly imbalanced classes
- No prior labels available

##Applications of anomaly detection
- Condition monitoring (Industrial maintenance) and failure prevention
- Fraud detection
- Intrusion detection
- Antivirus and antimalware tasks
- Data preparation(Identification of outliers)

#Chapter 22: Forecasting
A typical example of a forecasting problem would be: Given a set of ordered data points (such as sales data over a series of dates), we want to predict the next data points in the series (such as what sales will look like next week).

These orderable datasets can be time-series datasets, but they don't have to be—forecasting can be applied to other types of orderable sets as well.

##Types of forecasting algorithms

- ARIMA- Autoregressive Integrated Moving Average
- Multi-variate regression
- Prophet (Developed by Facebook- Suitable for datasets with high seasonality)
- ForecastTCN(Temporal Convulational Network)
- Recurrent Neural Networks (LSTMs etc)

