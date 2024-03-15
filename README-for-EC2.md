# EC2 Instance Setup on AWS with CloudFormation

## Overview
This repository contains a CloudFormation template for deploying an EC2 instance on AWS. The template automates the creation of an EC2 instance with specified instance type, security groups, and key pair. It provides a streamlined approach to deploying virtual servers on the AWS cloud platform.

## Prerequisites
Before deploying the EC2 instance using this CloudFormation template, ensure that you have:
- An AWS account with appropriate permissions to deploy CloudFormation stacks.
- Basic understanding of AWS EC2 instance concepts, including instance types and key pairs.

## Deployment Steps
To deploy the EC2 instance on AWS using this CloudFormation template, follow these steps:

1. Log in to the AWS Management Console.
2. Navigate to the CloudFormation service.
3. Click on the "Create stack" button.
4. Choose "Upload a template file" and select the provided CloudFormation template (ec2-instance-setup.yml).
5. Click "Next" to proceed with the stack creation.
6. Provide values for the required parameters, such as instance type and key pair name.
7. Review the configuration and click "Create stack" to initiate the deployment.
8. Wait for the stack creation process to complete. Once done, you will see the status as "CREATE_COMPLETE".

## Accessing the EC2 Instance
After the stack creation is complete, you can access the deployed EC2 instance using SSH or other remote access methods. Key resources created by the template include:
- EC2 instance with specified instance type and key pair
- Security groups for controlling inbound and outbound traffic

You can connect to the EC2 instance using the public DNS name or IP address provided in the CloudFormation stack outputs.

## Stopping and Cleaning Up
To stop or delete the deployed EC2 instance, follow these steps:

1. Log in to the AWS Management Console.
2. Navigate to the EC2 service.
3. Locate the EC2 instance created by this deployment.
4. Stop or terminate the instance as needed.
5. Optionally, delete the CloudFormation stack to remove all associated resources.

## Configuration
You can customize the deployment by modifying the CloudFormation template parameters, such as instance type and key pair name. Additionally, you can adjust the resource properties in the template to meet specific EC2 instance requirements.
