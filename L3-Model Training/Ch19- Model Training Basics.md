**Lesson 3:Model Training**

# Chapter 19- Model Training Basics

Models learn **parameters** from the data.

**Hyper-parameters** are the model parameters that are not learned from the data and are set before training.

Examples of hyperparameters 
- number of layers in a deep neural network
- number of clusters (such as in a k-means clustering algorithm)
- The learning rate of the model

A common approach is to take a best guess, train the model, and then tune the hyperparameters based on the model's performance.

Splitting the Data
- Training data -to learn the values for the parameters.
- Validation data- check the model's performance on the it and tune the hyperparameters until the model performs well with it.
- Test data- To do a final performance check on the data

# Chapter 20 - Model Training in Azure Machine Learning
## Causes

- **Workspace**- The centralized place for working with all the components of the machine learning process.
- **Experiment**- A container that helps you organize the model training process.
- **Model registry**- A service that provides snapshots and versioning for your trained models.
- **Compute instance** -A cloud-based workstation that gives you access to various development environments, such as Jupyter Notebooks.
- Run
- Model telemetry
