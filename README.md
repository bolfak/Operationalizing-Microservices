[![Bolfak](https://circleci.com/gh/bolfak/Operationalizing-Microservices.svg?style=svg)](https://github.com/bolfak/Operationalizing-Microservices)

## Project Overview

Predicts housing prices in Boston using a sklearn model that has been trained t according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.

The project can be run as a standalone python script and through Docker / Kubernetes

## Project Files
* [app.py](https://github.com/bolfak/Operationalizing-Microservices/blob/master/app.py)
The python flask app that makes the predictions

* [Dockerfile](https://github.com/bolfak/Operationalizing-Microservices/blob/master/Dockerfile)
Contains the instructions to build the Docker image

* [Makefile](https://github.com/bolfak/Operationalizing-Microservices/blob/master/Makefile)
The makefile to build the project

* [make_predictions.sh](https://github.com/bolfak/Operationalizing-Microservices/blob/master/make_predictions.sh)
A shell script to run a prediction against the model

* [requirements.txt](https://github.com/bolfak/Operationalizing-Microservices/blob/master/requirements.txt)
The python requirements file

* [run_docker.sh](https://github.com/bolfak/Operationalizing-Microservices/blob/master/run_docker.sh)
Builds and runs the docker container

* [run_kubernetes.sh](https://github.com/bolfak/Operationalizing-Microservices/blob/master/run_kubernetes.sh)
Runs the kubernetes cluster

* [upload_docker.sh](https://github.com/bolfak/Operationalizing-Microservices/blob/master/upload_docker.sh)
Uploads the docker image to the Duckerhub


## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
