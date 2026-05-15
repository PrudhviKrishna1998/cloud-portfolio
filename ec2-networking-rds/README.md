**# AWS EC2 Networking & Database Project **

This project is a personal portfolio website hosted on AWS EC2.

## 🚀 Features
- Deployed using AWS EC2
- Configured secure SSH access using key pairs
- Hosted using nginx web server
- Custom HTML/CSS resume website
  
## 🛠️ Technologies Used
- AWS EC2
- Linux (Ubuntu)
- nginx
- HTML/CSS
  
## ☁️ Deployment Architecture
- Application hosted on AWS EC2 instance
- Ubuntu Linux server used as compute environment
- nginx web server configured to serve static HTML
- SSH key-based authentication used for secure access
- Security Group configured to allow HTTP (80) and SSH (22)

Flow:
User Browser → HTTP Request → AWS EC2 (nginx) → index.html Response

## 📊 AWS Evidence
- EC2 instance launched and managed via AWS Console (:contentReference[oaicite:0]{index=0})
- Secure SSH access configured using key-pair authentication (.pem file)
- Security Groups configured to allow inbound HTTP (80) and SSH (22)
- Public IPv4 address assigned to EC2 instance for web access

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

## 🧩 Issues Faced
- EC2 instance not visible due to AWS region mismatch between root and IAM user
- Resolved by aligning both sessions to the same region (ap-south-1)

## 🔐 Private Subnet Setup
- Created a private subnet with no internet access
- Launched EC2 without public IP
- Accessed private EC2 securely via public EC2 (bastion host)

## 🔬 Networking Validation
Tested secure architecture by restricting direct SSH access to private EC2 and enabling access only via a public EC2 (bastion host).  
Verified internet isolation by confirming public EC2 has connectivity while private EC2 has no direct internet access.

## 🌐 NAT Gateway (Conceptual Understanding)
Learned how private EC2 instances can securely access the internet using a NAT Gateway without being exposed to inbound traffic.
- NAT Gateway is deployed in a public subnet with an Elastic IP
- Private subnet routes outbound traffic (0.0.0.0/0) to the NAT Gateway
- Enables outbound internet access while maintaining network isolation

## 🗄️ RDS (Relational Database Service)
- Created a MySQL RDS database using AWS RDS Free Tier  
- Configured secure connectivity between EC2 and RDS using Security Groups  
- Established secure EC2-to-RDS connectivity using MySQL client and Security Groups
- Executed SQL operations including database selection, table creation, data insertion, and querying

## 🌐 Live Website
http://13.223.50.206

## 📌 About Me
I am a Computer Engineering graduate with a strong foundation in networking (Cisco) and IT infrastructure. I am currently transitioning into cloud computing and actively building hands-on projects using AWS, Linux, and web server technologies.
