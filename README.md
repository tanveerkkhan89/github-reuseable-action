# Reusable GitHub Actions Workflows

This repository contains a set of reusable GitHub Actions workflows designed to simplify the automation of CI/CD processes for various projects. These workflows cover a range of operations, including infrastructure provisioning, application deployment, and code building.

## Overview of Workflows

### 1. Infrastructure Deployment
We have a workflow dedicated to deploying the required infrastructure on AWS, including the creation of a Virtual Private Cloud (VPC) and provisioning an Elastic Kubernetes Service (EKS) cluster.

- **VPC Setup**: Ensures secure and scalable networking on AWS.
- **EKS Cluster**: Automatically provisions an EKS cluster for container orchestration and management.

### 2. Helm Package Installation
Another workflow is responsible for managing Helm package installations. Helm charts are used to deploy applications onto the Kubernetes cluster, ensuring proper configuration and resource allocation.

- **Helm Charts**: Deploys applications using Helm charts for efficient and flexible application management on Kubernetes.

### 3. Infrastructure Destruction
For lifecycle management of your cloud resources, we have created a workflow to automate the destruction of the infrastructure. This ensures that once the resources are no longer needed, they are efficiently cleaned up.

- **Infrastructure Cleanup**: Destroys the provisioned AWS resources, including the VPC and EKS cluster.

### 4. Source Code Build
We also have a workflow that focuses on building the application source code. This step ensures that the application is properly compiled and ready for deployment.

- **Code Compilation**: Builds the source code for deployment using Maven or other build tools as per the project requirements.

## How to Use the Workflows

These workflows can be easily integrated into your project pipelines by referencing the appropriate `.yml` files. Each workflow is designed to handle a specific part of the deployment or development process, and they can be reused across multiple repositories.

By utilizing these reusable workflows, you can ensure consistency, modularity, and maintainability across your CI/CD pipelines.
