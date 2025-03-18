# MLFLOW Expertiment

import dagshub
dagshub.init(repo_owner='alihassanml', repo_name='mlflow-experiment', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)