**Lesson 2: Intro to Machine Learning**

# Chapter 6 - Common Types of Data
> Details of the type of data is important because the form and structure of the data fed into the machine learning algorithm  regarding:
>Choice of algorithms, value of hyperparameters and approaches to solve various problems.
## Numerical Data
Either integers or floats eg house prices
> All data fed into an algorithm ends up numeric despite its original form.

## Time Series
Series of numerical values that can be ordered, typically data collected over equally spaced points in time.
Can also be data ordered based on a non-datetime column.

**Examples:** Energy demand, realtime stocks performance

Complex cases such as speech data that gets transformed into time-based fequency values


## Categorical Data
Discrete and limited set of values

Most have small cardinality eg Gender. Some have high eg Location ID

## Text
Includes words, sentences eg news articles

**Challenge:** Transforming it into a numeric form appropriate for an ML algorithm is challenging.

## Images
Pictures, snapshots or full- streams of videos.

Not initially in numerical form but they will need to be transformed into RGB values, a set of numerical values ranging from 0 to 255, to be processed.
