# Project 1: Infrastructure as Code on AWS

**Deploy a containerized Nginx web server using Terraform and ECS Fargate**

---

## What This Creates

This project provisions the following AWS resources using Terraform:

- ECS Fargate cluster (serverless container hosting)
- ECS Service running an Nginx container
- CloudWatch Log Group for container logs
- Security Group to allow HTTP traffic (port 80)
- IAM roles for ECS task execution

---

## Prerequisites

- [Terraform](https://www.terraform.io/downloads.html)
- [AWS CLI](https://aws.amazon.com/cli/)
- AWS account (Free Tier is sufficient)

---

## Step-by-Step Deployment

### Step 1: Configure AWS CLI

```bash
aws configure
# Enter your Access Key, Secret Key, region (e.g. us-east-1), and output format (e.g. json)

aws sts get-caller-identity
# Confirms credentials are valid
