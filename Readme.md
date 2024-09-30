# Terraform AWS S3 Static Website Hosting

## Project Description
I developed an infrastructure to host a static website using Terraform and AWS S3, showcasing automated provisioning and deployment.

## Overview

## Key Components

- **Terraform IaC**: Defines and provisions AWS resources.
- **AWS S3 Bucket**: Stores and serves static website files.
- **Content Management**: Scripts for uploading and managing website content.

## Steps

1. **Set Up Development Environment**
   - I installed Terraform and the AWS CLI.
   - Configured AWS credentials:
     ```shell
     aws configure
     ```

2. **Define Website Content**
   - I placed `index.html` (and optionally `error.html`) in the Terraform directory.

3. **Terraform Configuration**
   - Created `provider.tf` with the AWS provider.
   - Initialized Terraform:
     ```shell
     terraform init
     ```

4. **Create S3 Bucket**
   - Defined the S3 bucket in `resource.tf`.
   - Applied the configuration:
     ```shell
     terraform apply -auto-approve
     ```

5. **Configure Bucket for Website Hosting**
   - Updated `resource.tf` with public access and website settings.
   - Applied the changes:
     ```shell
     terraform apply -auto-approve
     ```

6. **Output Website Endpoint**
   - Created `output.tf` to get the website URL.
   - Applied the configuration to retrieve the URL:
     ```shell
     terraform apply -auto-approve
     ```
