## Intro
The notebooks found here will help users learn how to configure and use AutoML in Azure Databricks. Please read all instructions carefully, as there are several pre-requisites.

**Note**: The 01_aml_getting_started.ipynb and 02_automated_ML.ipynb notebooks are part of the same solution, and should be run in the order indicated by the number prefixes. The notebook with the 01 prefix will configure your Azure Machine Learning workspace.
The 03_configuration.ipynb and 04_auto-ml-forecasting-a.ipynb are unrelated to notebooks 01 and 02, but are part of the same solution. They also should be run in order indicated by the numbers prefixes.

## Pre-requisites:
1. An Azure Databricks workspace. Follow this document to create a workspace: https://docs.azuredatabricks.net/getting-started/try-databricks.html

2. An Azure Databricks cluster. Follow this quickstart to get familiar with the UI and create a cluster: https://docs.azuredatabricks.net/getting-started/quick-start.html#quick-start

3. Install the following PyPi package on your cluster: azureml-sdk[automl_databricks]
This is necessary to use the auto_ml SDK on your cluster. 
**IMPORTANT** Make sure to RESTART your cluster after installing the SDK.
For details on how to install a library on your Databricks cluster, refer to this doc: https://docs.databricks.com/user-guide/libraries.html

4. **IMPORTANT**  For notebooks 01 and 02: If you haven't already ran the notebooks found in the 'sparkml' folder in this repo, please do that first. The output of these notebooks will be used for notebooks 01 and 02.
For notebooks 03 and 04: You will need the nyc_energy.csv dataset found in the datasets folder in this repo. There are various ways in which you can use this dataset in Databricks - for this lab, you can load the dataset into an Azure Blob container, and then mount the blob storage in Databricks.
To create an Azure Blob container, refer to this doc: https://docs.microsoft.com/en-us/azure/storage/blobs/storage-quickstart-blobs-portal
To mount blob storage in Azure Databricks, refer to this doc - scroll down to the section entitled "Mount Azure Blob Storage Containers with DBFS" https://docs.azuredatabricks.net/spark/latest/data-sources/azure/azure-storage.html#mount-azure-blob-storage-containers-with-dbfs

5. Ensure you have downloaded or cloned this repo, so that you have the files stored locally.

## Instructions:
1. Import the notebooks in this folder into Databricks. This documentation shows how to import notebooks: https://docs.databricks.com/user-guide/notebooks/notebook-manage.html
2. **PART 1: Notebooks 01 and 02**
Open 01_aml_getting_started, follow the instructions as per the notebook to configure your Azure Machine Learning workspace. Run the notebook.
Open 02_automated_ML.ipynb, and read the notes provided within the notebook. If you get any errors, please review the steps listed above, and ensure you have completed all pre-requisites.



**PLEASE NOTE**: I am not the owner/creator of any of the notebooks in this repo. Please see below for a list of the source repos containing the notebooks:
- Notebooks 01 and 02 -> https://github.com/Azure/LearnAI_Azure_ML/tree/master/presenter/notebooks/day_2
- Notebooks 03 and 04 -> https://github.com/FrancescaLazzeri/AutomatedMLEnergyForecast
