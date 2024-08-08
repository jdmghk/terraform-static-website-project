
# Hosting a Basic Website with Terraform and AWS S3

## Project Overview

In this project, I set up a simple and efficient way to host a basic website using Terraform and Amazon Web Services (AWS) S3. The main aim of this project is to show how to automatically create and deploy a website without much hassle.

## Terraform Configuration Overview

The Terraform configuration for this project includes the following resources:

### AWS Provider
- Defining the AWS provider and specifying the region where the website will be hosted.

### S3 Bucket
- Creating an S3 bucket to store the website files.

### S3 Bucket Versioning
- Enabling versioning on the S3 bucket to keep track of changes to the website files.

### S3 Bucket Ownership and Access Control
- Configuring the bucket's ownership and access control settings to ensure the website is publicly accessible.

### S3 Bucket Website Configuration
- Setting the bucket as a website-hosting bucket by configuring the necessary properties, such as the index document and error document.

### S3 Bucket Policy
- Creating an S3 bucket policy to allow public read access to the website files.

### Uploading Website Files
- Using the `aws_s3_object` resource to upload the website files (HTML, CSS, JavaScript, etc.) to the S3 bucket.

### CloudFront Distribution (optional)
- Creating an AWS CloudFront distribution and configuring it to use the S3 bucket as the origin, for added performance and reliability.

### DNS Configuration (optional)
- Setting up DNS records to point to the S3 bucket or the CloudFront distribution, if a custom domain is used.

By leveraging Terraform and AWS S3, this project demonstrates a simple and efficient way to automatically create and deploy a basic website, without the need for manual configuration or setup.
