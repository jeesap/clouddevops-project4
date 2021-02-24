[![CircleCI](https://circleci.com/gh/jeesap/project4.svg?style=svg)](https://circleci.com/gh/jeesap/project4) 

## Summary of the project

A pre-trained sklearn model has been given as part of this project . Sklearn has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. Project goal is to operationalize this working, machine learning microservice using kubernetes, which is an open-source system for automating the management of containerized applications. In this project following tasks are expected to be done.

Test project code using linting
Complete a Dockerfile to containerize this application
Deploy containerized application using Docker and make a prediction
Improve the log statements in the source code for this application
Configure Kubernetes and create a Kubernetes cluster
Deploy a container using Kubernetes and make a prediction
Upload a complete Github repo with CircleCI to indicate that code has been tested


## Setup the Environment

Create a virtualenv and activate it

$python3 -m venv ~/.devops
$source ~/.devops/bin/activate

Run make install to install the necessary dependencies

$make install


 ## Running scripts
 
To run app.py in standalone: 

$python app.py

To run app.py in Docker: 

$./run_docker.sh

To run app.py in Kubernetes: 

$./run_kubernetes.sh

To make a prediction, open a separate tab or terminal window and run

$./make_prediction.sh

To upload an image to docker, run below script

$./upload_docker.sh

## Files included

1).circleci - CircleCI config scripts
2)model_data - ML model related data (model, csv data)
3)output_txt_files - Project output files (docker, kubernetes)
4)docker_out.txt - run_docker.sh output
5)kubernetes_out.txt - run_kubernetes.sh output
6)app.py - Python web application
7)Dockerfile - Docker image config
8)make_prediction.sh - Make prediction HTTP call script
9)Makefile - make file (install, test, lint steps)
10)requirements.txt - Web application dependencies to be installed (python, libraries)
11)run_docker.sh - Run docker container script
12)run_kubernetes.sh - Script to run kubernetes pod for the web app 
13)upload_docker.sh - Script to upload docker image to docker hub script 


