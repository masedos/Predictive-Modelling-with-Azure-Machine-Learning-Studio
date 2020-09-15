# Predictive-Modelling-with-Azure-Machine-Learning-Studio
Predictive Modelling with Azure Machine Learning Studio

![Evaluation results](https://github.com/masedos/Predictive-Modelling-with-Azure-Machine-Learning-Studio/blob/master/Evaluation_results.PNG)


###To access the dataset

#### Weather Dataset.csv
from azureml import Workspace
ws = Workspace(
    workspace_id='db68414bc7024ab0875349b59784056b',
    authorization_token='2saJtX+Ib+DRlcVMgRG/d00twJXCmsZPK//K0sXD/nFkQ1VvoR5CqjIW06m/3T3MprPWw4hyOiwjDuUdO0E+hQ==',
    endpoint='https://studioapi.azureml.net'
)
ds = ws.datasets['Weather Dataset.csv']
frame = ds.to_dataframe()

#### Flight Delays Data.csv
from azureml import Workspace
ws = Workspace(
    workspace_id='db68414bc7024ab0875349b59784056b',
    authorization_token='2saJtX+Ib+DRlcVMgRG/d00twJXCmsZPK//K0sXD/nFkQ1VvoR5CqjIW06m/3T3MprPWw4hyOiwjDuUdO0E+hQ==',
    endpoint='https://studioapi.azureml.net'
)
ds = ws.datasets['Flight Delays Data.csv']
frame = ds.to_dataframe()
