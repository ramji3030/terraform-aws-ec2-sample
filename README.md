# Terraform AWS EC2 Sample

A sample Terraform project demonstrating AWS EC2 instance provisioning with automation.

## Overview

This project provides a simple example of how to use Terraform to provision and manage AWS infrastructure, specifically an EC2 instance. It serves as a learning resource for Infrastructure as Code (IaC) practices.

## Prerequisites

Before running this project, ensure you have:

- [Terraform](https://www.terraform.io/downloads.html) installed (v1.0+)
- [AWS CLI](https://aws.amazon.com/cli/) configured with appropriate credentials
- An AWS account with necessary permissions to create EC2 instances

## Project Structure

```
terraform-aws-ec2-sample/
├── main.tf          # Main Terraform configuration
├── README.md        # This file
└── .gitignore      # Git ignore file for Terraform
```

## Usage

### 1. Clone the Repository

```bash
git clone https://github.com/ramji3030/terraform-aws-ec2-sample.git
cd terraform-aws-ec2-sample
```

### 2. Configure AWS Credentials

Ensure your AWS credentials are configured:

```bash
aws configure
```

### 3. Initialize Terraform

```bash
terraform init
```

### 4. Plan the Deployment

```bash
terraform plan
```

### 5. Apply the Configuration

```bash
terraform apply
```

### 6. Clean Up Resources

When you're done, destroy the resources to avoid charges:

```bash
terraform destroy
```

## What This Project Creates

- An EC2 instance in the default VPC
- A security group allowing SSH access
- Tags for resource identification

## Configuration Details

The `main.tf` file includes:

- AWS provider configuration
- Security group with SSH access
- EC2 instance using Amazon Linux 2 AMI
- Output values for instance details

## Customization

You can customize the deployment by modifying variables in `main.tf`:

- Instance type (default: t2.micro)
- AMI ID (default: latest Amazon Linux 2)
- Tags and naming

## Learning Resources

- [Terraform Documentation](https://www.terraform.io/docs/)
- [AWS Provider Documentation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)
- [Terraform Best Practices](https://www.terraform.io/docs/cloud/guides/recommended-practices/)

## License

This project is provided as-is for educational purposes.

## Contributing

Feel free to submit issues and enhancement requests!
