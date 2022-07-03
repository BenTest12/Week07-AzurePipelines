![image](https://bootcamp.rhinops.io/images/cicd-pipeline.gif)
# CI-CD PROJECT

## Introduction
This Weeks project cosists of the following tools:
 - [Azure DevOps](dev.azure.com)
 - [Terraform](https://www.terraform.io/)
 - [Ansible](https://www.ansible.com/)
 
## Project Overview
Using these tools , i orchestrated a build pipeline for sela group's nodejs weight app by creating 2 environments.

2 environments (Staging and Production) which consists of 3 virtual machines in a scaleset , behind a load balancer , with a managed PostgreSQL as a DB.

These environments were built using Terraform code , [Link to the code](https://github.com/BenTest12/week07_terraform) , 
And provisioned by my ansible controller.

The whole pipeline ran on my AzureDevops pipelines , Please refer to my [Azure-Pipelines.yml file.](https://github.com/BenTest12/Week07-AzurePipelines/blob/main/azure-pipelines.yml)

![](https://bootcamp.rhinops.io/images/week-6-envs.png)

## Goals
Create an Azure DevOps Organization

Create a CI Pipeline using Azure Pipelines (preferably using yaml)

Use Azure Artifacts to store your build Artifacts

Create a CD Pipeline using Azure Release Pipelines

Configure your CD pipeline to deploy to Staging using Continuous Deployment

Configure your CD pipeline to deploy to Production using Continuous Deployment

CI pipeline should trigger automatically on every commit

## Expected Result

Full CI/CD pipeline that automates the process of building and deploying the application in a pre existent infrastructure

In case of making a change to the code and pushing it, it will be automatically deployed to the Staging environment

Deployment to production must consist of a single click operation (manual approval)
