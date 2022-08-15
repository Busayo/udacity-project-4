
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

##How to run app
* Create a virtual environment with python3 -m venv venv
* Source the virtual environment: source venv/bin/activate
* Run make install to install the necessary dependencies

## Then

* Standalone: python app.py
* Run in Docker: ./run_docker.sh
* Run in Kubernetes: ./upload_docker.sh && ./run_kubernetes.sh
* Having the application running in container, in a separate terminal run ./make_prediction.sh
