[![Bolfak](https://circleci.com/gh/bolfak/Operationalizing-Microservices.svg?style=svg)](https://github.com/bolfak/Operationalizing-Microservices)

## Project Overview

Predicts housing prices in Boston using a sklearn model that has been trained t according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.

The project can be run as a standalone python script and through Docker / Kubernetes

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
