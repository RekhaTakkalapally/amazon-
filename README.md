# AWS S3 Static Website Deployment using Terraform

This project demonstrates how to deploy a **static website (Amazon Clone demo)** on **Amazon Web Services (AWS)** using **Terraform Infrastructure as Code (IaC)**.

Terraform automatically provisions an **Amazon S3 bucket**, configures **static website hosting**, and deploys website files such as **HTML and CSS**.  
This allows infrastructure to be created, managed, and destroyed programmatically instead of manually configuring resources in the AWS console.

---

## Features

- Infrastructure provisioning using **Terraform**
- Static website hosting using **AWS S3**
- Public bucket policy configuration
- Automated deployment of website files
- Infrastructure managed using **Infrastructure as Code (IaC)**

---

## Technologies Used

- AWS S3
- Terraform
- HTML
- CSS
- Git
- GitHub
- GitHub Actions (CI/CD)

---

## Architecture

User → Internet → AWS S3 Bucket → Static Website Hosting → Website Output

Terraform provisions the infrastructure and uploads the website files automatically.  
Amazon S3 static website hosting serves the website through a public endpoint.
## Architecture Diagram

![Architecture Diagram](screenshots/s3-static-website-hosting.png)

---
## Website Output

![Website Output](screenshots/website-output.png)

---

## Terraform Deployment Steps

### 1 Initialize Terraform
terraform init


### 2 Review Infrastructure Plan


terraform plan


### 3 Deploy Infrastructure


terraform apply


Terraform will create the required AWS resources and output the **S3 website URL**.

---

## CI/CD Pipeline

This project includes a **GitHub Actions CI pipeline** that automatically checks Terraform code whenever changes are pushed to the repository.

The pipeline performs the following steps:

- Terraform initialization
- Terraform format validation
- Terraform plan execution

---

## Prerequisites

Before running this project, make sure you have:

- AWS Account
- Terraform installed
- AWS CLI installed
- AWS credentials configured

Configure AWS credentials:


aws configure


---

## Cleanup

To remove all resources created by Terraform:


terraform destroy


This command deletes the S3 bucket and associated infrastructure.

---

## Author

**Rekha Takkalapally**

DevOps | Cloud | AWS | Terraform
