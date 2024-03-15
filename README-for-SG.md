# Security Group Setup

## Description
This CloudFormation template sets up security groups in AWS to control inbound and outbound traffic to EC2 instances.

## Parameters
- **SSHLOC:** Specifies the IP address range that can be used to SSH to the EC2 instances.
  
## Resources
- **sgPING:** Security group to allow ICMP traffic for ping testing.
- **sgWEB:** Security group to allow SSH access (port 22) and HTTP (port 80) traffic.

## Usage
1. Ensure you have an existing VPC.
2. Deploy this CloudFormation template and specify the required parameters.
3. The security groups will be created with the specified rules.

## Notes
- The `sgWEB` security group allows SSH and HTTP traffic from any IP address by default. Make sure to adjust the rules as per your security requirements.
- Make sure to import the VPC details if deploying this template in a different stack.
