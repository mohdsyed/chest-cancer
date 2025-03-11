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



#MLflow on AWS
MLflow on AWS Setup:

    Login to AWS console.
    Create IAM user with AdministratorAccess
    Export the credentials in your AWS CLI by running "aws configure"
    Create a s3 bucket
    Create EC2 machine (Ubuntu) & add Security groups 5000 port

Run the following command on EC2 machine

sudo apt update

sudo apt install python3-pip

sudo apt install pipenv

sudo apt install virtualenv

mkdir mlflow

cd mlflow

pipenv install mlflow

pipenv install awscli

pipenv install boto3

pipenv shell


## Then set aws credentials
aws configure


#Finally 
mlflow server -h 0.0.0.0 --default-artifact-root s3://syed-store

#open Public IPv4 DNS to the port 5000


#set uri in your local terminal and in your code 
export MLFLOW_TRACKING_URI=http://ec2-3-88-229-63.compute-1.amazonaws.com:5000/