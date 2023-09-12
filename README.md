# SafeSlothSweep API

**Introduction:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Machine learning models for malware categorization are to be deployed within the framework of this project. There are three tasks in this project. The first aim is to use the Ember open-source dataset, EMBER-2017 v2, to train a deep neural network to categorize PE files as malicious or benign. Endgame Malware Benchmark for Research, or EMBER, is a sizable dataset made up of labeled and unlabeled samples of features extracted from PE header files from binaries. On https://github.com/endgameinc/ember, you may find more information regarding the dataset.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Deploying the model to the cloud and developing an endpoint (API) for the model are the subject of the second task. Create a client consisting just of a Python script that imports a PE file and categorizes it as malicious or benign as the last task. 'Anaconda3-2020.02-Windows-x86_64.exe' is used as the sample to execute the built client. Any PE file may be used; there are no limitations.

[**Task 1: Model Building:**](https://github.com/parindi/SafeSlothSweep/blob/main/AISec_Task%201_Model%20Building.ipynb) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data is first extracted, vectorized, and preprocessed in this task. Then Keras is used to create a deep neural network architecture. The retrieved data is used to train, validate, and test the model. To improve model performance, hyperparameters are adjusted. The weights of the model are preserved. Finally, a method is developed that takes in a PE file and determines whether it is benign or malicious.

[**Task 2: Model Deployment to Cloud:**](https://github.com/parindi/SafeSlothSweep/blob/main/AISec_Task_2_Model_Deployment.ipynb) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AWS Sagemaker is the cloud service utilized in this project. To deploy the saved model to Sagemaker, it is uploaded and loaded. Thus, an endpoint had been created.

[**Task 3: Client Creation:**](https://github.com/parindi/SafeSlothSweep/tree/main/AISec_Task%203_Client%20Creation%20%26%20Execution)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In order to complete this task, a Python program must be written that takes a PE file, transforms it into a feature vector suitable with the model, runs the feature vector via the cloud API, and presents the results (i.e., Malware or Benign, or probability of each).

