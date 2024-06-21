# What is ML ops?

ML Ops is a set of principles and practices to standardize and streamline  the machine learning lifecycle management.

# What is CI/CD workflow.?
A CI/CD workflow for ML pipelines can be described with the following two concepts:

* Pipeline continuous integration, which consists of automated building and testing
* Pipeline continuous delivery, which consists of automated pipeline deployment for continuous training and delivery of ML models

# Pipeline CI [[ref]](https://www.iguazio.com/glossary/ci-cd-for-machine-learning/#:~:text=A%20CI%2FCD%20workflow%20for,and%20delivery%20of%20ML%20models)
The pipeline CI process consists of three stages: 
* development,
* build, and
* testing

The ML pipeline and its components are built, tested, and packaged for delivery when changes are made on the source code repository (usually Git-based). 

During the development process, you iteratively experiment with new ML algorithms and modeling approaches where the experiment steps are orchestrated and tracked. You can then select an appropriate model and push the source code of the ML pipeline to the source code repository.

When changes are detected in the source code repository, it triggers a Git-based CI/CD workflow that starts the automated CI/CD pipeline process. During the build stage, the ML pipeline and its components are built with its dependencies in the form of packages, container images, and executables.

# Pipeline CD [[ref]](https://www.iguazio.com/glossary/ci-cd-for-machine-learning/#:~:text=A%20CI%2FCD%20workflow%20for,and%20delivery%20of%20ML%20models)

During the Pipeline continuous delivery (CD) process, the CI/CD pipeline continuously deploys new ML pipeline implementations that in turn perform continuous training (CT) of ML models for prediction.

During CT of the ML model in the pipeline CD process, the deployed ML pipeline is automatically triggered for model retraining in production based on triggers from the live ML pipeline environment. Model retraining could be triggered either per a schedule, due to model performance degradation, or due to significant changes in data distributions of the features used for prediction (also known as concept drift). The trained ML model is then automatically deployed as a model prediction service as part of the model CD process.

Continuous monitoring of your model’s performance based on live data in production enables the detection of model performance degradations and concept drift so that the CT pipeline can be automatically triggered to retrain and deploy an updated ML model based on more recent data.