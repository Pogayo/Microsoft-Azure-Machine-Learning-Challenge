**Lesson 3:Model Training**

# Chapter 12 - Introducing Features


- **Features**- The columns of a data table or matrix; also known as fields, or variables.
- **Feature engineering**- The process through which we create new features.
- **Feature selection**- The process through which we choose which features will be used in the model training process.
- **The curse of dimensionality** - The phenomenon in which an ML algorithm is not capable of coping with very large numbers of features.
- **dimensionality reduction** -Decreasing the number of features

>Data wrangling is an iterative process where you do some data transformation then check the results and come back to the process to make improvements.

# Chapter 13 - Feature Engineering

Feature engineering manipulates existing features to create new features with the goal of improving the performance of the model

It can be performed in multiple places, such as the data source and during model training

Classical ML depends on feature engineering much more than deep learning.

## Common Feature engineering tasks
- Aggregation - Count, Median, Distinct count, sum
- Part of - Extracting a part of a certain data structure eg- Extracting a day from date
- Binning - Grouping instances by an attrubute then performing aggregations on them
- Flagging - Deriving a boolean (0/1 or True/False) value for each entity
- Frequency based - Calculating various frequencies
- Embedding (Feature Learning)
- Deriving by examples - aim to learn values of new features using existing features

Text embedding is the process of transforming text/natural language into numerical formats.

Common approaches for text are:
- Text frequency
- Inverse Document Frequency
- Word embedding

Not much engineering is required for image data as the features are learned naturally in the case of neural networks.