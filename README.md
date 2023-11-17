# Deploying_a_Cluster_of_Web_Servers With Terraform

This Terraform configuration automates the deployment of an Auto Scaling Group behind an Application Load Balancer on AWS.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Configuration Details](#configuration-details)
- [Resources Created](#resources-created)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Overview

This Terraform script sets up an Auto Scaling Group (ASG) in AWS behind an Application Load Balancer (ALB). It creates necessary security groups, configures the load balancer, establishes listeners and rules, and manages auto-scaling configurations.

## Prerequisites

Before running this Terraform script, ensure you have:

- Valid AWS credentials configured locally or using environment variables.
- Terraform installed (version 1.0.0 or higher).

## Usage

1. Clone this repository.
2. Navigate to the directory containing the Terraform files.
3. Initialize Terraform:

    ```bash
    terraform init
    ```

4. Review and modify `variables.tf` to adjust any required settings.
5. Execute the Terraform plan:

    ```bash
    terraform plan
    ```

6. Apply changes:

    ```bash
    terraform apply
    ```

## Configuration Details

### Terraform Version

This script requires Terraform version 1.0.0 or higher.

### Provider Configuration

Provider: AWS
- Region: `us-east-2`

### Resources Created

- Application Load Balancer (ALB)
- Auto Scaling Group (ASG)
- Launch Configuration
- Security Groups
- Load Balancer Listeners and Rules

## Troubleshooting

- **Error in Terraform Execution**: Check the error logs and ensure proper AWS permissions and configurations are set.
- **Resource Not Created**: If certain resources are not created, verify the Terraform scripts for any configuration issues.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
