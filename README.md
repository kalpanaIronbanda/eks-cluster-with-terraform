EKS Cluster with Terraform
---------------------------
This repository contains the necessary code and configurations to deploy an Amazon Elastic Kubernetes Service (EKS) cluster using Terraform. The infrastructure provisioning and management tasks can be automated with Terraform, enabling easy creation and management of EKS clusters.

Prerequisites
--------------
Before getting started, ensure that you have the following prerequisites:

AWS Account: You need an active AWS account with appropriate permissions to create and manage resources like VPC, EKS clusters, and IAM roles.

Terraform: Install Terraform on your local machine. You can download it from the official website: Terraform Downloads.

AWS CLI: Install and configure the AWS Command Line Interface (CLI) on your local machine.

Getting Started
----------------
To deploy an EKS cluster using Terraform, follow these steps:

Clone this repository: 

		git clone https://github.com/kalpanaIronbanda/eks-cluster-with-terraform.git

Change into the repository directory: 

		cd eks-cluster-with-terraform

Configuration
-----------------

The repository includes a variables.tf file where you can modify the desired configuration parameters for your EKS cluster. 

you can change the region in that file
region: The AWS region where the cluster will be created.


Deployment
--------------

To deploy the EKS cluster, run the following commands:

Initialize the Terraform project: 

		terraform init

Preview the changes: 

		terraform plan

Deploy the EKS cluster: 

		terraform apply

Terraform will prompt you to confirm the changes before deploying the infrastructure. Review the changes carefully and type "yes" when prompted.

The deployment process may take several minutes to complete. Once finished, Terraform will output the necessary information to access and manage your EKS cluster.

Accessing the EKS Cluster
----------------------------

To access and manage your EKS cluster, you can use the AWS CLI or other Kubernetes management tools such as kubectl. Refer to the official AWS documentation for detailed instructions on how to configure and interact with EKS clusters: Amazon EKS Documentation

Clean Up
------------

To destroy the resources created by Terraform and clean up the infrastructure, run the following command:

		terraform destroy

Review the resources to be destroyed, and type "yes" when prompted. This will delete the EKS cluster and associated resources.

Please note that this action is irreversible and will permanently delete all the resources created by this Terraform configuration.
