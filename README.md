# Cloud Infrastructure as Code (IaC)

A comprehensive collection of IaC templates and scripts for deploying scalable cloud architectures on AWS.

## Architecture

This repository contains code to provision a highly available 3-tier web application architecture:
- **VPC Configuration**: Public and private subnets across multiple Availability Zones
- **Compute**: Auto Scaling Groups with EC2 instances behind an Application Load Balancer
- **Database**: RDS PostgreSQL Multi-AZ deployment
- **Storage**: S3 buckets for static assets with CloudFront CDN

## Tools Used

- **Terraform**: Main infrastructure provisioning
- **Ansible**: Configuration management and application deployment
- **Docker**: Containerization of microservices
- **GitHub Actions**: CI/CD pipeline for automated testing and deployment

## Usage

1. Initialize Terraform:
   ```bash
   cd terraform
   terraform init
   ```

2. Plan and Apply:
   ```bash
   terraform plan -out=tfplan
   terraform apply tfplan
   ```

