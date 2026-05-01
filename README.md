# Cloud Portfolio Website

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

## 🔐 IAM Learning Notes
- Learned IAM user vs root user access differences
- Understood region-based resource visibility in AWS
- Configured IAM group with EC2 permissions

  ## 🧩 Issues Faced
- EC2 instance not visible due to AWS region mismatch between root and IAM user
- Resolved by aligning both sessions to the same region (ap-south-1)

## 🌐 Live Website
http://13.223.50.206

## 📌 About Me
I am a Computer Engineering graduate with a strong foundation in networking (Cisco) and IT infrastructure. I am currently transitioning into cloud computing and actively building hands-on projects using AWS, Linux, and web server technologies.
