**Lesson 2: Intro to Machine Learning**

# Chapter 28 - Approaches to Machine Learning

There are three main approaches to machine learning:


## 1. Supervised learning
Learns from data that contains both the inputs and expected outputs (e.g., labeled data). Common types are:

- Classification: Outputs are categorical.
- Regression: Outputs are continuous and numerical.
- Similarity learning: Learns from examples using a similarity function that measures how similar two objects are.
- Feature learning: Learns to automatically discover the representations or features from raw data.
- Anomaly detection: A special form of classification, which learns from data labeled as normal/abnormal.
## 2. Unsupervised learning
Learns from input data only; finds hidden structure in input data.

- Clustering: Assigns entities to clusters or groups.
- Feature learning: Features are learned from unlabeled data.
- Anomaly detection: Learns from unlabeled data, using the assumption that the majority of entities are normal.
## 3.Reinforcement learning
Learns how an agent should take action in an environment in order to maximize a reward function.
 >Reinforcement learning is an active process where the actions of the agent influence the data observed in the future, hence influencing its own potential future states. In contrast, supervised and unsupervised learning approaches are passive processes where learning is performed without any actions that could influence the data.


# Chapter 29 - The Trade-Offs

## Bias vs. Variance
>Bias measures how inaccurate the model prediction is in comparison with the true output. It is due to erroneous assumptions made in the machine learning process to simplify the model and make the target function easier to learn. High model complexity tends to have a low bias.

>Variance measures how much the target function will change if different training data is used. Variance can be caused by modeling the random noise in the training data. High model complexity tends to have a high variance.

As a general trend, parametric and linear algorithms often have high bias and low variance, whereas non-parametric and non-linear algorithms often have low bias and high variance

> prediction error = Bias error + variance + error + irreducible error

Bias error + variance - Model error

irreducible error- Data collection error
>The goal of training machine learning models is to achieve low bias and low variance. The optimal model complexity is where bias error crosses with variance error.

## Overfitting vs. Underfitting
Overfitting refers to the situation in which models fit the training data very well, but fail to generalize to new data.

Underfitting refers to the situation in which models neither fit the training data nor generalize to new data.

### How to reduce overfitting
- k-fold cross-validation: it split the initial training data into k subsets and train the model k times. In each training, it uses one subset as the testing data and the rest as training data.
- hold back a validation dataset from the initial training data to estimatete how well the model generalizes on new data.
- simplify the model. For example, using fewer layers or less neurons to make the neural network smaller.
- use more data.
- reduce dimensionality in training data such as PCA: it projects training data into a smaller dimension to decrease the model complexity.
- Stop the training early when the performance on the testing dataset has not improved after a number of training iterations.