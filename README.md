DEVOPS ASSESSMENT
===

DevOps - Take Home Assessment

Part I Deliver Terraform Code

Part II Deliver Small App for K8S and a Helm Chart

Part III Setup an AKS cluster and Azure SQL Database 

Part IV GitHub Action for II and III

You can attempt all or any of the parts you’re best conversant with this will give us an insight into your area of specialization  during our review.

Part I
===
## Deliver Terraform Code

Create a Helm repository using Azure Blob Storage (search on the internet for instructions) The Azure Blob Storage should be created using Terraform.

Once the bucket is ready, push some example charts into the repository You will find on the internet Helm s3 plugins that help interact with s3 as a Helm repository.

Part II
===
## Deliver Small App for K8S and a Helm Chart

1. Create a simple HTTP app in the language of your choice that upon query returns the contents of the  Azure Blob Storage in JSON format.

2. Create a Dockerfile for the application.

3. Create a Helm chart to deploy the application to AKS cluster.

Considerations:

2 Take into account proper configuration of the application via the Helm chart as it requires details for the Azure Blob Storage, address etc.

- Consider adding a mechanism to validate the application’s health - To develop and deploy your application you can use the k8s cluster in part IV.

The final result of the application, its Dockerfile and its Helm chart should all be present in a single GitHub repository.

Part III
===
## Setup an AKS cluster and Azure SQL Database 
Write a terraform code to deploy an AKS cluster running on two nodes that should  be deployed into a new Azure Virtual Network.


Part IV
===
## Helm Chart GitHub Action
Create a Github action that upon merge to a certain branch packages the application’s Helm chart and pushes it to the S3 repository

