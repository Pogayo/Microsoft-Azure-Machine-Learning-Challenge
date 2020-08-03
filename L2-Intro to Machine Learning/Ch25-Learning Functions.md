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