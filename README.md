# Terraform + LocalStack EC2 Example

This is a sample project that provisions an EC2 instance on LocalStack using Terraform. It's intended for testing and learning infrastructure-as-code workflows without needing a real AWS account.

## Prerequisites

- Terraform
- LocalStack (running via pipx or Docker)
- AWS CLI (configured to work with LocalStack)
- Python 3 and pipx (for managing LocalStack if installed via pipx)

## Usage

1. Initialize the Terraform project:
   ```bash
   terraform init
   ```

2. Preview the changes Terraform will make (optional but recommended):
   ```bash
   terraform plan
   ```

3. Apply the changes:
   ```bash
   terraform apply
   ```

4. Or apply without prompt:
   ```bash
   terraform apply -auto-approve
   ```

## Notes

- Make sure LocalStack is running before applying the configuration.
- The Terraform backend and provider are configured to connect to LocalStack rather than AWS.
- State and cache files (like `.terraform`, `terraform.tfstate`) are excluded from version control.
