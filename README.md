## MLFlow Experement

import dagshub
dagshub.init(repo_owner='soumenmaity3', repo_name='dagshub_with_mlflow_exper', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)