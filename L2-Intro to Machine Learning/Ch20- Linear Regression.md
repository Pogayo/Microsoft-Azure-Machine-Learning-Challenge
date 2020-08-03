**Lesson 2: Intro to Machine Learning**

# Chapter 20- Linear Regression
>Linear regression is an algorithm that uses a straight line (or plane) to describe relationships between variables.

Linear regression is all about finding the line that best fits the data.
## Linear Regression in Machine Learning

>y=mx+b

In algebraic terms we refer  to 
- **m** as the **coefficient** of x or simply the **slope** of the line
- **b** the **y-intercept**. 

In machine learning, typically the y-intercept IS referred to as the **bias**. The equation is represented using different variables, as in:

>y = B_0 + B_1*x

The letters are different and the order has been changed, but it is exactly the same equation. 
In ML this basic equation for a line is used  for **simple linear regression**.

## Multiple Linear Regression
Where there is more than one input variable, we see something like this:

y = B_0 + B_1*x_1 + B_2*x_2 + B_3*x_3 ... + B_n *x_n

We call it **multiple linear regression**. The visualization of multiple linear regression is no longer a simple line, but instead a plane in multiple dimensions.

## Training a Linear Regression Model
To "train a linear regression model" means to learn the coefficients and bias that best fit the data.

### The Cost Function
When we make a prediction using the line, we expect the prediction to have some **error**.

The process of finding the best model is essentially a process of finding the coefficients and bias that minimize this error using a cost function. There are many cost functions you can choose from to train a model and the resulting error will be different depending one which cost function you choose. The most commonly used cost function for linear regression is the **root mean squared error (RMSE)**

### Preparing the data

- **Linear assumption:** The relationship between the input variables and the output variable needs to be a linear relationship. If the raw data does not follow a linear relationship, transform your data appropriately. For example, if your data has an exponential relationship, you can use log transformation.
- **Remove collinearity:** When two variables are collinear, they can be modeled by the same line or are at least highly correlated; in other words, one input variable can be accurately predicted by the other.  Having highly correlated input variables will make the model less consistent. Perform a correlation check among input variables and remove highly correlated input variables.
- **Gaussian (normal) distribution:** Linear regression assumes that the distance between output variables and real data (called residual) is normally distributed. If this is not the case in the raw data,transform the data so that the residual has a normal distribution.
- **Rescale data:** Linear regression is very sensitive to the distance among data points. Normalize or standardize the data.
- **Remove noise:** Linear regression is very sensitive to noise and outliers.Clean the data.
