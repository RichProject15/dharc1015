To deploy the network setup on AWS using this CloudFormation template, follow these steps:

1. Log in to the AWS Management Console.
2. Navigate to the CloudFormation service.
3. Click on the "Create stack" button.
4. Choose "Upload a template file" and select the provided CloudFormation template (network-setup.yml).
5. Click "Next" to proceed with the stack creation.
6. Provide values for the required parameters, such as VPC CIDR block and public subnet CIDR block.
7. Review the configuration and click "Create stack" to initiate the deployment.
8. Wait for the stack creation process to complete. Once done, you will see the status as "CREATE_COMPLETE".

Accessing the Network Resources
After the stack creation is complete, you can access and manage the deployed network resources using the AWS Management Console or AWS CLI. Key resources created by the template include:
- Virtual Private Cloud (VPC)
- Internet Gateway (IGW)
- Public Subnet
- Route Tables

You can view and manage these resources through the VPC Dashboard and Route Tables section in the AWS Management Console.

Stopping and Cleaning Up
To stop or delete the deployed network resources, follow these steps:

1. Log in to the AWS Management Console.
2. Navigate to the CloudFormation service.
3. Select the stack created by this deployment.
4. Click on "Delete stack" and confirm the deletion.
5. Wait for the stack deletion process to complete. Once done, all associated resources will be removed from your AWS account.
