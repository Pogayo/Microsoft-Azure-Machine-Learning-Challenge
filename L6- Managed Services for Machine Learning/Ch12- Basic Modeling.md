**Lesson 6: Managed Services**

# Chapter 2 - Basic Modelling

**Experiments**: is a generic context for handling runs. Think about it as a logical entity you can use to organize your model training processes.
             
**Runs**:model training runs are what you use to build the trained model. A run contains all artifacts associated with the training process, like output files, metrics, logs, and a snapshot of the directory that contains your scripts.

##Run confiigurations
- Set of instructions that specify how a script should be run in a specified compute environment
- Include a wide set of behaviour definitios

##Models

a model is a piece of code that takes an input and produces output. To get a model, we start with a more general algorithm. By combining this algorithm with the training data—as well as by tuning the hyperparameters—we produce a more specific function that is optimized for the particular task we need to do. Put concisely:
>Model = algorithm + data + hyperparameters

Training is an iterative process

How to deploy Python models as a web service
- Register the model in the model registry
- Image is deployed in AKS
- mODELS stored within Azure Container regisry
- Client sent an HTTP request with input data
- Web service extracts the question and sends it to the model
- The result is sent back

## Model registry
- Keeps track of all your trained models in azure ML workspace
- Models are identified by name and version
- When you register a model, you can provide additional metadata tags
- You can't delete a model that is being used in active deployment
- When you deploy a model using the Designer, it registers the model automatically for you.
- When you use the SDK, you can register the model with code

#Chapter 15: Advanced Modelling
As the process of building your models becomes more complex, it becomes more important to get a handle on the steps to prepare your data and train your models in an organized way. In these scenarios, there can be many steps involved in the end-to-end process, including:

- Data ingestion
- Data preparation
- Model building & training
- Model deployment.

These steps are organized into **machine learning pipelines**.


##MLOps
The discipline that deals with the application of DevOps principles to projects that have atleast one data science component

- Automate end to end ML lifecycle
- Monitor ML processes
- Capture traceability data

#Chapter 17: Operationalizing models
After you have trained your machine learning model and evaluated it to the point where you are ready to use it outside your own development or test environment, you need to deploy it somewhere. Another term for this is operationalization.

##Typically Model Deployment
- Get the model file
- Create a scoring script(.py)
- Optionally create a schema file describing  the web service input(.json)
- Create real-time scoring web-services
- Call the web-service from your application
- Repeat the process each time you retrain a model

Deploy the model on Azure Kubernetes service if you need the following capabilities:
- fast response times
- Auto scaling
- Hardware acceleration eg GPU, FPGA

Use Azure Container Instance if:
- You need to quickly deploy and validate the model
- testing the model under development



##Real- time inferencing
Making decisions on new data on-demand is called real-time inferencing.

Options for deploying real time inferencing model
- Create manuallly using Azure ML studio
- Programmatically using Azure ML SDK


##Batch inferencing
Unlike real-time inferencing, which makes predictions on data as it is received, batch inferencing is run on large quantities (batches) of existing data. Typically, batch inferencing is run on a recurring schedule against data stored in a database or other data store
###When to use batch inferencing?
- No need for real-time
- Inferencing results can be persisted
- Post processing or analysis of predictions is required
- Inferencing is complex

##Lambda architecure
- A combination of real-time and batch
- Predictions are made at two different speeds
    * Hot path- makes the predictions in real-time
    * Cold path-makes predictions in batch fashion, usually on a predefined schedule
- Batch and real-time inferences are stored in the serving layer for reporting and auditing
- Hot and cold path converge at the analytic client application
