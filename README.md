# chest-cancer
## for daghub
import dagshub
dagshub.init(repo_owner='mohdsyed', repo_name='chest-cancer', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

## mlflow 
MLFLOW_TRACKING_URI=https://dagshub.com/mohdsyed/chest-cancer \
MLFLOW_TRACKING_USERNAME=mohdsyed \
MLFLOW_TRACKING_PASSWORD=a0379f651cd1e51c6a41f5a884c88500d2347652 \

```bash

export MLFLOW_TRACKING_URI=https://dagshub.com/entbappy/chest-Disease-Classification-MLflow-DVC.mlflow

export MLFLOW_TRACKING_USERNAME=entbappy 

export MLFLOW_TRACKING_PASSWORD=6824692c47a369aa6f9353c5b10041d5c8edbcef0

```

## Doghub token:   a0379f651cd1e51c6a41f5a884c88500d2347652
export MLFLOW_TRACKING_URI=https://dagshub.com/mohdsyed/chest-cancer
export MLFLOW_TRACKING_USERNAME=mohdsyed
export MLFLOW_TRACKING_PASSWORD= a0379f651cd1e51c6a41f5a884c88500d2347652
