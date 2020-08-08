**Lesson 4:Supervised and unsupervised learning**

# Chapter 3- Classification

A classification problem occurs when the expected output are categorical(discrete).

## Categories of classification problems
- Binary Classification - Classify medical test results as "positive" or "negative".
- Multiclass single label classification - Classify an image as one (and only one) of five possible fruits.
- Multiclass multilabel classification - Classify music as belonging to multiple groups (e.g., "upbeat", "jazzy", "pop"). 

## common types of classification problems 
- Classification on tabular data: The data is available in the form of rows and columns, potentially originating from a wide variety of data sources.
- Classification on image or sound data:
- Classification on text data

## More specific examples
- Computer Vision
- Speech recogntion 
- Sentiment analysis
- Biometric identification
- Anomaly detection

## Binary Classifiers

Algorithm | Characteristics
--------|--------
Two-class Suport Vector Machine |Under 100 features. linear model
Two-class  Averaged Perceptron| Fast training time, linear model
Two-class Decision Tree | Accurate, fast training times
Two-class Logistic regression| Fast training times, linear model
Two-class  Boosted Decision Tree|Accurate, Fast training, large memory footprint
Two-class neural network| Accurate, long training times

## Multi-class Classifiers

Algorithm | Characteristics
--------|--------
Multi--class Decision Forest | Accurate, fast training times
Multi--class Logistic regression| Fast training times, linear model
Multi--class  Boosted Decision Tree|Non-parametricFast training, scalable
Multi--class neural network| Accurate, long training times
One-vs- All Multi-class Depends on the underlying two-class classifier

# Chapter 7- Multi-class Algorithms

##Multi-class Algorithms Hyperparameters

Algorithm |Hyperparameter
--------|--------
Multi--class Logistic regression| Optimization tolerance, regularization weight
Multi--class Decision Forest | Resampling method, No of decision trees, max depth, no of random splits, min number of samples per leaf node
Multi--class neural network| Number of hidden nodes, learning rate, no of learning iterations

