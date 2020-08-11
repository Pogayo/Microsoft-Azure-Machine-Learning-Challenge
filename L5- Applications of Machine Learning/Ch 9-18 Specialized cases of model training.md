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

Note: use the same vocabulary as in the trai set for the test set
- 