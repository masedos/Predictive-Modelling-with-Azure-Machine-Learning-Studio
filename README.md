# Predictive Modelling with Azure Machine Learning Studio

Welcome to Project: Predictive Modelling with Azure Machine Learning Studio. This is a project-based course which should take approximately 2 hours to complete. Before diving into the project, please take a look at the course objectives and structure:

## Course Objectives
In this course, we are going to focus on three learning objectives:
<br>
- Build a predictive model using Azure ML Studio.
- Demonstrate a working knowledge of setting up experiments on Azure ML Studio.
- Operationalise machine learning work flows with Azure's drag-and-drop modules.
<br>
By the end of this course, you will be able to train and evaluate a predictive model on Azure Machine Learning Studio, all without writing a single line of code! You will predict flight delays using weather data provided by the US Bureau of Transportation Statistics and the National Oceanic and Atmospheric Association (NOAA).

## Project Structure
- Task 1: Introduction and Setup Instructions
- Task 2: Importing the Data Sets
- Task 3: Scrubbing Missing Values
- Task 4: Eliminating Target Leaks
- Task 5: Conversion to Categorial Features
- Task 6: Preparing Features to be Joined with Weather Data
- Task 7: Preprocessing the Weather Dataset
- Task 8: Joining Both Datasets
- Task 9: Training and Evaluating the Model
<br>

![Evaluation results](https://github.com/masedos/Predictive-Modelling-with-Azure-Machine-Learning-Studio/blob/master/Evaluation_results.PNG)


### To access the dataset

#### Weather Dataset.csv
'''
from azureml import Workspace
ws = Workspace(
    workspace_id='db68414bc7024ab0875349b59784056b',
    authorization_token='2saJtX+Ib+DRlcVMgRG/d00twJXCmsZPK//K0sXD/nFkQ1VvoR5CqjIW06m/3T3MprPWw4hyOiwjDuUdO0E+hQ==',
    endpoint='https://studioapi.azureml.net'
)
ds = ws.datasets['Weather Dataset.csv']
frame = ds.to_dataframe()
'''
#### Flight Delays Data.csv
'''
from azureml import Workspace
ws = Workspace(
    workspace_id='db68414bc7024ab0875349b59784056b',
    authorization_token='2saJtX+Ib+DRlcVMgRG/d00twJXCmsZPK//K0sXD/nFkQ1VvoR5CqjIW06m/3T3MprPWw4hyOiwjDuUdO0E+hQ==',
    endpoint='https://studioapi.azureml.net'
)
ds = ws.datasets['Flight Delays Data.csv']
frame = ds.to_dataframe()
'''
