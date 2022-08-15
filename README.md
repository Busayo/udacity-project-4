
[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Busayo/udacity-project-4/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Busayo/udacity-project-4/tree/master)

## Udacity Cloud DevOps Nanodegree Project 4 : Operationalize a Machine Learning Microservice API

In this project, we will apply all previous skills gained to operationalize a Machine Learning Microservice API.

File Summary:

* .circleci - for circleCI testing and link
* model_data - contains data used to train program
* output_txt_files - contains log output when when the run_docker.sh and run_kubernetes.sh files are called.
* Dockerfile: contains commands used to create and run image
* Makefile: commands used to run program
* app.py: main Flask program 
* run_docker.sh - contains commands to run docker cotainer locally
* run_kubernetes.sh - contains commands used to run K8s pod locally
* make_prediction.sh - used to run predictions

## How to setup environment (on AWS Cloud9 and locally)
* Create a virtual environment with python3 -m venv venv
* Source the virtual environment: source venv/bin/activate
* Run make install and make lint to install the necessary dependencies and to check for errors in Dockerfile

## To run on AWS Cloud9

* Run a local container and test if app is successfully launched - ./run_docker.sh
* Run prediction - ./make_prediction.sh
* Upload Docker image to remote repository - ./upload_docker.sh
* Start minikube cluster - run minikube start
* Deploy container with Minikube - ./run_kubernetes.sh
* Run prediction - ./make_prediction.sh
* You can also run python script alone - python app.py

## To run the app locally
* Make sure Docker, minikube and kubectl are installed on local machine.
* Same steps above. Make sure to edit the ./run_kubernetes.sh file to match local minikube configuration and image created in the upload_docker.sh file. The run_kubernetes.sh file uses kubectl to create the required pods.



