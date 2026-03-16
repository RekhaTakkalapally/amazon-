AWS S3 Static Website Deployment using Terraform

This project demonstrates how to deploy a static website (Amazon Clone demo) on Amazon Web Services (AWS) using Terraform Infrastructure as Code (IaC).

Terraform is used to automatically provision an Amazon S3 bucket, configure static website hosting, and deploy the website files such as HTML and CSS. This approach allows infrastructure to be created, managed, and destroyed programmatically instead of manually configuring resources in the AWS console.

Features

Infrastructure provisioning using Terraform

Static website hosting using AWS S3

Public bucket policy configuration

Automated deployment of website files

Infrastructure managed using Infrastructure as Code (IaC)

Technologies Used

AWS S3

Terraform

HTML

CSS

Git & GitHub

GitHub Actions (CI/CD)

Project Structure
aws-s3-static-website-terraform
│
├── main.tf        # Terraform configuration for S3 bucket
├── variables.tf   # Terraform input variables
├── outputs.tf     # Output values such as website URL
│
├── index.html     # Main website page
├── error.html     # Error page
├── style.css      # Website styling
│
├── Static Website Amazon/
│   └── website-output.png
│
└── README.md
Architecture

This project follows a simple architecture for hosting a static website on AWS.

User → Internet → AWS S3 Bucket → Static Website Hosting → Website Output

The static website files are stored in an Amazon S3 bucket. Terraform provisions the infrastructure and configures the bucket for website hosting. When a user accesses the website URL, the content is served directly from the S3 bucket through the static website endpoint.

Website Output

Below is the deployed website example.



Terraform Deployment Workflow

Terraform is used to create and manage the AWS infrastructure.

Step 1 — Initialize Terraform
terraform init
Step 2 — Review Infrastructure Plan
terraform plan
Step 3 — Deploy Infrastructure
terraform apply

Terraform will create the required AWS resources and display the S3 website URL in the output.

CI/CD Pipeline

This project includes a GitHub Actions CI pipeline that automatically checks Terraform code whenever changes are pushed to the repository.

The workflow performs:

Terraform initialization

Terraform formatting validation

Terraform execution plan

This helps ensure that infrastructure code follows best practices before deployment.

Prerequisites

Before running this project, ensure you have:

AWS Account

Terraform installed

AWS CLI installed

AWS credentials configured

Configure AWS credentials using:

aws configure
Cleanup

To delete all resources created by Terraform:

terraform destroy

This command removes the S3 bucket and associated infrastructure.

Learning Outcomes

This project demonstrates:

Infrastructure as Code using Terraform

Static website hosting using AWS S3

Cloud infrastructure automation

Basic DevOps workflow with GitHub

Author

Rekha Takkalapally

DevOps | Cloud | AWS | Terraform
