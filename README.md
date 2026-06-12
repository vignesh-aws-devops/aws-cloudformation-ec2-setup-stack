# aws-cloudformation-ec2-setup-stack

## 🚀 Experimenting with AWS CloudFormation | AWS Native Infrastructure as Code (IaC) Service | EC2 Infrastructure Deployment via CloudFormation Stack

## 🟢 What is AWS CloudFormation?

AWS CloudFormation is an Infrastructure as Code (IaC) service that enables users to define, provision, and manage AWS infrastructure through templates and stack-based deployments.

CloudFormation Stacks act as a single unit for managing infrastructure and can contain multiple AWS resources required for networking, compute, storage, CI/CD pipelines, DevOps workflows, and complete cloud architectures. CloudFormation automatically manages resource dependencies and enables infrastructure to be created, updated, and deleted in a consistent and repeatable manner.

Created a YAML template that provisions a complete AWS networking environment along with an EC2 instance, demonstrating how infrastructure can be deployed consistently and repeatedly through code.

## ✅ Key Concepts Implemented

- Provisioned an Amazon VPC with DNS support and hostnames enabled
- Created a Public Subnet with automatic public IP assignment
- Attached an Internet Gateway (IGW) to provide internet connectivity to the VPC
- Configured a Route Table and associated it with the Public Subnet to route internet-bound traffic through the Internet Gateway
- Created a Security Group allowing SSH (22) and HTTP (80) access
- Launched an EC2 Instance (t3.micro) within the Public Subnet and associated it with the Security Group
- Configured CloudFormation Outputs to retrieve the EC2 Instance Public IP after deployment

## 🏗️ Architecture Diagram

![AWS CloudFormation EC2 Architecture](AWS%20CFN%20EC2.png)

## ⚙️ CloudFormation Workflow & Commands Used

- `aws cloudformation validate-template` – Validates the CloudFormation template before deployment
- `aws cloudformation deploy` – Creates the CloudFormation Stack and provisions the infrastructure
- `aws cloudformation describe-stacks` – Retrieves stack details and outputs
- `aws cloudformation describe-stack-events` – Monitors stack creation events and resource status
- `aws cloudformation delete-stack` – Deletes the CloudFormation Stack and all associated resources

## 💡 Takeaways & Learnings

- Infrastructure can be provisioned consistently through reusable CloudFormation templates
- CloudFormation Stacks simplify the lifecycle management of AWS resources
- Infrastructure as Code reduces manual effort and configuration drift
- Automated deployments improve consistency, scalability, and reliability
- Understanding VPCs, Subnets, Route Tables, Internet Gateways, Security Groups, and EC2 is essential for cloud automation
- CloudFormation provides a strong foundation for building larger and more complex AWS architectures through code

## 🔷 Source Code

https://github.com/vignesh-aws-devops/aws-cloudformation-ec2-setup-stack/tree/main

## 🟢 Let's Connect!

If you're passionate about DevOps or curious about AWS and cloud automation, let's connect! I'd love to exchange ideas, discuss strategies, or collaborate on exciting projects.
