**Lesson 2: Responsible AI**

# Chapter 2 - Managed Services for Machine Learning
Managed services for machine learning provide a ready-made environment that is pre-optimized for your machine learning development.

##Conventional Machine Learning
- Lengthy installation and set up process
- Expertise too configure hardware
- Fair amount of troubleshooting
##Managed services approach
- Very little setup
- Easy configuration for any needed hardware


## Examples of compute resources
- Training clusters
- Inference clusters
- Compute instances
- Attached compute
- Local compute

## Other Services
- Notebooks gallery
- Automated Machine Learning configurator
- Pipeline designer
- Datasets and datastores
- Experiments manager
- Pipelines manager
- Models registry
- Endpoint manager

#Chapter 4: Compute Resources
A **compute target** is a designated compute resource or environment where you run training scripts or host your service deployment.

##1. Training Compute
Computes used for training:
- Training clusters - multiple nodes
- Compute instance
- Localcompute

###Training clusters
- Used for training and batch inferencing
- Single or multinode cluster
- Can autoscale each time you submit a run
- Support for both GPU and CPU resources

##2. Inferencing compute
Real-time inference  | Batch inferencing/scoring
---------|-----------
Make inference for each new row, usually in real time|Make inference to multiple rows called batches
Web service ideal although others such as deployement to an iot device available | Any compute resource
For deployement- Azure kubernetes Service| 
- Dedicated type of compute called inferencing cluster for real time inferencing

Trained models can be packaged in containers.
###Compute targets for specialized deployments
1. Azure functions
2. Azure IoT edge
3. Azure Data Box Edge

