**Lesson 2: Intro to Machine Learning**

# Chapter 25 - Learning Functions

A machine learning algorithm is a process for learning, and models a specific representations that we train using data.
ML algorithms aim to learn a target function (f) that describes the mapping between data input variables (X) and an output variable (Y).

>Y = f(X)

The core goal is to learn a useful transformation of the input data that gets us closer to the expected output.

Since the process extrapolates from a limited set of values, there will always be an error *e* which is independent of the input data (X) such that:

>Y = f(X) + eY=f(X)+e

The variable *e* is called **irreducible error** because no matter how good we get at estimating the target function (f), we cannot reduce this error.


Irreducible error | Model error
------------ | ------------
Caused by the data collection process—such as when we don't have enough data or don't have enough data features. | Is generated from the model
Cannot be reduced | Can be reduced during the model learning process.

# Chapter 26 - Parametric and Non-parametric Algorithms

ML algorithms can be divided into two **parametric** and **nonparametric** based on the assumptions about the *shape* and *structure* of the function they try to learn.

Parametric | Non-parametric
------------ | ------------
Make assumptions about the mapping function and have a fixed number of parameters.  | Do not make assumptions regarding the form of the mapping function.
We are selecting the form of the function and then learning its coefficients using the training data.  |  They are free to learn any functional form from the training data.
Simpler and easier to understand; easier to interpret the results  |Overfitting the training data is a risk; overfitting makes it harder to explain the resulting predictions
Faster when talking about learning from data | Slower to train
Less training data required to learn the mapping function, working well even if the fit to data is not perfect | More training data is required
Highly constrained to the specified form of the simplified function | High flexibility- they are capable of fitting a large number of functional forms
Limited complexity of the problems they are suitable for | Power by making weak or no assumptions on the underlying function
Poor fit in practice, unlikely to match the underlying mapping function. | High performance
Logistic regression, Linear regression | Decision trees, KNN

# Chapter 27 - Classical ML vs Deep Learning
>Deep learning is a subset of machine learning
>
Classical ML algorithms | Deep Learning algorithms 
------------ | ------------
Based on classical mathematical algorithms, such as linear regression, logistic regression, decision tree, SVM | Based on neural networks
More suitable for small data | Better support for big data
Easier to interpret outcomes |  Difficult to explain outcomes| 
Does not require large computational power, cheaper to perform, can run on low-end machines  | Require significant computational power
Difficult to learn large datasets | Complex features can be learned
Require feature engineering | Better accuracy, compared to classical ML
Difficult to learn complex functions | Suitable for high complexity problems