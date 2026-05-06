## 🌐 Static Website Hosting using S3

This project demonstrates hosting a static website using Amazon S3.

### 🚀 Features
- Hosted HTML website using S3
- Configured public access using bucket policy
- Enabled static website hosting

## 🔐 IAM Access Control
* Created IAM users with different permission levels (admin-user and s3-user)
* Assigned full access to admin-user and limited read-only access to s3-user
* Verified access by successfully using S3 and receiving “Access Denied” for restricted EC2 actions
* Demonstrated principle of least privilege and IAM policy enforcement

## 🔐 IAM Roles
* Created an IAM role to allow EC2 to securely access S3 without using access keys
* Attached the role with S3 read-only permissions to the EC2 instance
* Verified access by running AWS CLI commands from EC2 and successfully listing S3 buckets
* Demonstrated secure service-to-service authentication using IAM roles

### 🌍 Live Website
https://prudhvi-portfolio-s3.s3.us-east-1.amazonaws.com/index.html
