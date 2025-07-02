###mlflow ###
import dagshub
dagshub.init(repo_owner='Naveenkumar-2007', repo_name='mlflow', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)