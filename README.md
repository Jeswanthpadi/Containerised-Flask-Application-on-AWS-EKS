# Containerised Flask Application on Amazon EKS

## Overview

This project focused on containerising a Python Flask application and deploying it to Amazon Elastic Kubernetes Service (EKS).

Docker was used to package the application, while Amazon Elastic Container Registry (ECR) was used to store the container image. Kubernetes resources were configured to deploy and expose the application within the EKS cluster.

The project also used AWS Boto3 and the Kubernetes Python client to interact with cloud and cluster resources programmatically.


## Architecture

The deployment workflow involved the following components:

- **Python Flask:** Application development and backend functionality.
- **Docker:** Containerisation of the Flask application.
- **Amazon ECR:** Storage of the Docker container image.
- **Amazon EKS:** Managed Kubernetes environment for running the application.
- **EKS Node Group:** Provided compute capacity for Kubernetes workloads.
- **Kubernetes Deployment:** Managed the application pod configuration.
- **Kubernetes Service:** Configured access to the deployed application.
- **AWS Boto3:** Programmatic interaction with AWS resources.
- **Kubernetes Python Client:** Programmatic creation of Kubernetes resources.
- **kubectl:** Inspection and management of Kubernetes resources.

## Technologies Used

- Python
- Flask
- Docker
- Amazon Web Services (AWS)
- Amazon ECR
- Amazon EKS
- Kubernetes
- Boto3
- Kubernetes Python Client
- kubectl

## Implementation

### 1. Flask Application Development

Developed a Python Flask application and prepared its dependencies for containerisation.

### 2. Docker Containerisation

Created a Dockerfile using a Python base image, installed the required dependencies, and packaged the Flask application into a container image.

### 3. Amazon ECR Repository

Used AWS Boto3 to create an Amazon ECR repository and prepared the application image for storage in the container registry.

### 4. Amazon EKS Environment

Set up the EKS cluster and node group to provide the Kubernetes environment required to run the containerised application.

### 5. Kubernetes Deployment

Used the Kubernetes Python client to configure Kubernetes Deployment and Service resources. The Deployment referenced the application image stored in Amazon ECR.

### 6. Application Verification

Used kubectl to inspect Kubernetes resources, check pod and service status, and verify application access through port forwarding.

## Deployment Workflow

The overall workflow followed these steps:

1. Develop the Flask application.
2. Build the Docker image.
3. Create an ECR repository.
4. Push the container image to Amazon ECR.
5. Set up the EKS cluster and node group.
6. Configure Kubernetes Deployment and Service resources.
7. Inspect the deployment using kubectl.
8. Access and verify the application through port forwarding.

## Key Learning Outcomes

- Containerising Python applications using Docker.
- Understanding Amazon ECR and container image management.
- Working with Amazon EKS and Kubernetes.
- Creating Kubernetes Deployment and Service resources.
- Using Boto3 to interact with AWS services.
- Using the Kubernetes Python client for resource configuration.
- Inspecting Kubernetes workloads and verifying application access with kubectl.

## Project Scope

This was a team-based academic project demonstrating containerisation, AWS-managed Kubernetes deployment, and programmatic resource configuration. It focused on deploying and verifying a Flask application rather than implementing a complete production-grade Kubernetes platform.

Jeswanth Naidu Padi

[GitHub](https://github.com/Jeswanthpadi) · [LinkedIn](https://www.linkedin.com/in/jeswanthnaidupadi/)
