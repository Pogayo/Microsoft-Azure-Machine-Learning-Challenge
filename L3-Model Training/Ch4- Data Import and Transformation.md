**Lesson 3:Model Training**

# Chapter 4 - Data Import and Transformation


**Data wrangling** is the process of cleaning and transforming data to make it more appropriate for data analysis. 
- Explore the raw data and check the general quality of the dataset.
- Transform the raw data, by restructuring, normalizing, and cleaning the data. For example, this could involve handling missing values and detecting errors.
- Validate and publish the data.



>Data wrangling is an iterative process where you do some data transformation then check the results and come back to the process to make improvements.


# Chapter 7 -Managing Data 
Datastore in Azure Machine Learning is a layer of abstraction that provides an isolation from the various supported data storages in Azure.

Datasets are resources for exploring, transforming, and managing data in Azure ML. A dataset is essentially a reference that points to the data in storage. 

Datastore | Dataset
-------- | --------
Answers the question, "how do I securely connect to the data in my Azure storage?"| Answers the question, "how do I get access to specific data files?"
Keeps connection information internal, so it is not exposed in scripts.| Points to specific files in your underlying storage that you want to use in your ML experiments.

## The Data Access Workflow

The steps of the data access workflow are:

1. Create a datastore so that you can access storage services in Azure.
2. Create a dataset, which you will subsequently use for model training in your machine learning experiment.
3. Create a dataset monitor to detect issues in the data, such as data drift.

Data Drift - The situation where the input data that you are feeding into your model changes overtime. It can be problematic for model accuracy. 

You can set up dataset monitors to detect data drift and other issues in your data. When data drift is detected, you can have the system automatically update the input dataset so that you can retrain the model and maintain its accuracy.