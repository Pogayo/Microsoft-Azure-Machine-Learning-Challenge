**Lesson 2: Intro to Machine Learning**

# Chapter 15- The Tools for  ML

Made up of 3 main components:
1. Libraries:  A library is collection of pre-written (and compiled) code that you can make use of in your own project.
Examples - Numpy, Pandas, Kera, Pytorch, TensorFlow
2. Development Environment: A development environment is a software application (or sometimes a group of applications) that provide a whole suite of tools designed to help you (as the developer or machine learning engineer) build out your projects.
Examples - Jupyter Notebooks(Open-source tool that can combine code, markdown, and visualizations together in a single document), Visual studio code
3. Cloud services. A cloud service is a service that offers data storage or computing power over the Internet. In the context of machine learning, you can use a cloud service to access a server that is likely far more powerful than your own machine, or that comes equipped with machine learning models that are ready for you to use.


##  End-to-end with Azure
To train and test models, you can use: 
 - Azure Data Science Virtual Machine, 
 - Azure Databricks
 - Azure Machine Learning Compute
 - SQL server ML services 
 
To deploy models, you can use:
 - Azure Kubernetes Service(AKS)
 - Azure container instance(ACI)
 - Core ML
 
# Chapter 16- Libraries for  ML

##  Core Framework and Tools

- **Python** is a popular high-level programming language that is easy to use and has wide wide support within popular machine learning platforms, coupled with a large catalog of ML libraries.
- **Pandas** is an open-source Python library designed for analyzing and manipulating data. It is particularly good for working with tabular data and time-series data.
- **NumPy** is a Python library that provides support for large, multi-dimensional arrays of data, and has many high-level mathematical functions that can be used to perform operations on these arrays.


## Machine Learning and Deep Learning

- **Scikit-Learn** is a Python library designed to be integrated with other scientific and data-analysis libraries, such as NumPy, SciPy, and matplotlib.
- **Apache Spark** is an open-source analytics engine that is designed for cluster-computing and that is often used for large-scale data processing and big data.
- **TensorFlow** is a free, open-source software library for machine learning built by Google Brain.
- **Keras** is a Python deep-learning library. It provide an Application Programming Interface (API) that can be used to interface with other libraries, such as TensorFlow, in order to program neural networks. Keras is designed for rapid development and experimentation.
- **PyTorch** is an open source library for machine learning, developed in large part by Facebook's AI Research lab. It is known for being comparatively easy to use, especially for developers already familiar with Python and a Pythonic code style.

## Data Visualization

- **Plotly** is a company that provides a number of different front-end tools for machine learning and data science—including an open source graphing library for Python.
- **Matplotlib** is a Python library designed for plotting 2D visualizations. It can be used to produce graphs and other figures that are high quality and usable in professional publications. Is used by a number of other libraries and tools, such as SciKit Learn and Seaborn . 
- **Seaborn** is a Python library based on matplotlib, but provides a more high-level interface and has additional features for making visualizations more attractive and informative.
- **Bokeh** is an interactive data visualization library that generates visualizations in HTML and JavaScript. This allows for web-based visualizations that can have interactive features.

# Chapter 16- Cloud Services

A typical cloud service for machine learning provides support for managing the core assets involved in machine learning projects.
## Core Asset Management
Feature | 	Description
------------ | ------------
Datasets	| Define, version, and monitor datasets used in machine learning runs.
Experiments / Runs| 	Organize machine learning workloads and keep track of each task executed through the service.
Pipelines| 	Structured flows of tasks to model complex machine learning flows.
Models | 	Model registry with support for versioning and deployment to production.
Endpoints| 	Expose real-time endpoints for scoring as well as pipelines for advanced automation.

Machine learning cloud services also need to provide support for managing the resources required for running machine learning tasks:
## Resource Management
Feature	| Description
------------ | ------------
Compute	| Manage compute resources used by machine learning tasks.
Environments | 	Templates for standardized environments used to create compute resources.
Datastores  | 	Data sources connected to the service environment (e.g. blob stores, file shares, Data Lake stores, databases).

## A Brief Intro to Azure Machine Learning

Below are features of the Azure ML Workspace-A centralized place to work with all the artifacts you create.

Feature	| Description
------------ | ------------
Automated ML|	Automate intensive tasks that rapidly iterate over many combinations of algorithms, hyperparameters to find the best model based on the chosen metric.
Designer|	A drag-and-drop tool that lets you create ML models without a single line of code.
Datasets|	A place you can create datasets.
Experiments	|A place that helps you organize your runs.
Models|	A place to save all the models created in Azure ML or trained outside of Azure ML.
Endpoints|	A place stores real-time endpoints for scoring and pipeline endpoints for advanced automation.
Compute|	A designated compute resource where you run the training script or host the service deployment.
Datastores|	An attached storage account in which you can store datasets.