**Lesson 2: Intro to Machine Learning**

# Chapter 12- Two Perspectives in ML

>Computer Science - We are using input features to create a program that can generate the desired output.

>Statisical - We are trying to find a mathematical function that, given the values of the independent variables can predict the values of the dependent variables.


## Computer Science Perspective

A row is callled an **entity** or an **observation** about an entity or  **instance**, in the sense that a row may be considered a single example (or instance) of data.

A column might be referred to as a **feature** or **attribute** which describes the property of an entity.

When there are multiple input variables, the row can be described as  **input vector**

## Statistical Perspective

In statistics, you'll the data is described in terms of independent variables and dependent variables.

From a statistical perspective, the machine learning algorithm is trying to learn a hypothetical function (f) such that:

>Output Variable = f(Input Variables)
>
Typically, the independent variables are the input, and the dependent variables are the output. Thus, the above formula can also be expressed as:

>Dependent Variable = f(Independent Variables)

In shorthand notation
>Y = f(X)

In the case of multiple input variables, X would be an **input vector**, meaning that it would be composed of multiple individual inputs (e.g. (908721, Guess, Blue, 789, 45.33)). In this case, the individual inputs are denoted with a subscript, as in X1, X2, X3 etc.

