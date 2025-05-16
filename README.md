
# Terraform LocalStack EC2

This project demonstrates how to provision EC2 instances on LocalStack using Terraform. It allows testing AWS infrastructure locally without real AWS credentials.

## Prerequisites

- Terraform installed
- LocalStack running locally
- AWS CLI configured for LocalStack
- Python virtual environment with required packages installed

## Usage

1. Activate your virtual environment:
   ```bash
   source .venv/bin/activate
   ```
2. Initialize Terraform:
   ```bash
   terraform init
   ```
3. Apply Terraform configuration:
   ```bash
   terraform apply -auto-approve
   ```
4. Check EC2 instances via AWS CLI:
   ```bash
   aws ec2 describe-instances --endpoint-url=http://localhost:4566
   ```
