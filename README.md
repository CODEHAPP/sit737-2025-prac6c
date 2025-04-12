
# SIT737-2025-Prac6C - Cloud Native Application Development

## Overview

This repository contains the code and configuration files for **SIT737-2025-Prac6C** project, which is part of the Cloud Native Application Development course. In this part of the project, we continue interacting with a Kubernetes cluster to deploy and manage a microservice application. The application is built with **Node.js** and **Docker**.

## Prerequisites

Before you can work with this project, make sure you have the following tools installed:

- **[Git](https://git-scm.com/)** - for version control
- **[Node.js](https://nodejs.org/en/download/)** - to run and develop the Node.js application
- **[Docker](https://www.docker.com/get-started)** - to build and manage Docker containers
- **[Kubernetes](https://kubernetes.io/)** - the platform for deploying and managing containers
- **[Kubectl](https://kubernetes.io/docs/tasks/tools/)** - the command-line tool for interacting with Kubernetes clusters

## Project Structure

## Instructions for Running the Application

1. **Clone the repository**:
   ```bash
   git clone https://github.com/CODEHAPP/sit737-2025-prac6c.git
   cd sit737-2025-prac6c
2.Build the Docker image: In the project directory, run:
docker build -t nodejs-kube-app .
3.Deploy the application to Kubernetes: After building the Docker image, use the following command to deploy it to your Kubernetes cluster:
kubectl apply -f kubernetes/deployment.yaml
kubectl apply -f kubernetes/service.yaml
4.Verify the deployment: You can check the status of your application using:
kubectl get pods
kubectl get services
5.Access the application: Forward the port from your Kubernetes service to your local machine:
kubectl port-forward service/nodejs-kube-app 3000:3000
Then open your browser and navigate to http://localhost:3000 to access the application.

Updating the Application

1.Build a new Docker image with a new tag:
docker build -t nodejs-kube-app:v2 .
Update the Kubernetes deployment configuration to use the new image tag by modifying the deployment.yaml file.

2.Apply the updated deployment:
kubectl apply -f kubernetes/deployment.yaml


