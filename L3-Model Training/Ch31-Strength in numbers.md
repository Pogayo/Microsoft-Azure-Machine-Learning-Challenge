**Lesson 3:Model Training**

# Chapter 31 - Strength in numbers
 You can often get better results by training multiple models or using multiple algorithms and in some way capturing the collective results.
 
 There are two main approaches to this: 
 - Ensemble learning and
 - Automated machine learning. 
 
 ## Ensemble learning
 
 ensemble learning combines multiple machine learning models to produce one predictive model. 
 
 They are of three main types:
 
 ### 1.Bagging or bootstrap aggregation
 
 - Helps reduce overfitting for models that tend to have high variance (such as decision trees)
 - Uses random subsampling of the training data to produce a bag of trained models.
 - The resulting trained models are homogeneous
 The final prediction is an average prediction from individual models
 
 ### 2. Boosting
 
 - Helps reduce bias for models.
 -  In contrast to bagging, boosting uses the same input data to train multiple models using different hyperparameters.
 - Boosting trains model in sequence by training weak learners one by one, with each new learner correcting errors from previous learners
 - The final predictions are a weighted average from the individual models

 ###3. Stacking
 
- Trains a large number of completely different (heterogeneous) models
- Combines the outputs of the individual models into a meta-model that yields more accurate predictions

## Strength in Variety: Automated ML
Automated machine learning  automates many of the iterative, time-consuming, tasks involved in model development (such as selecting the best features, scaling features optimally, choosing the best algorithms, and tuning hyperparameters). 

Automated ML allows data scientists, analysts, and developers to build models with greater scale, efficiency, and productivity—all while sustaining model quality.
