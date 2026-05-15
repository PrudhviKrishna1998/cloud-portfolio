# 📈 AWS Monitoring, Load Balancing & Auto Scaling

This project demonstrates monitoring, high availability, and automatic scaling of AWS infrastructure using Amazon CloudWatch, Application Load Balancer (ALB), and Auto Scaling Groups (ASG).

## 🚀 Features
- Monitored EC2 performance using Amazon CloudWatch
- Configured CloudWatch alarms for CPU utilization
- Integrated SNS email notifications for alerts
- Configured an Application Load Balancer (ALB)
- Distributed traffic across multiple EC2 instances
- Created Auto Scaling Group for dynamic EC2 scaling
- Tested automatic scaling using CPU stress simulation

## 🛠️ Technologies Used
- Amazon EC2
- Amazon CloudWatch
- Amazon SNS
- Application Load Balancer (ALB)
- Auto Scaling Group (ASG)
- Ubuntu Linux

## ☁️ Deployment Architecture

Flow:

User Traffic  
↓  
Application Load Balancer  
↓  
EC2 Instances  
↓  
CloudWatch Monitoring  
↓  
Auto Scaling Response

## 📊 CloudWatch Monitoring
- Monitored EC2 instance metrics using Amazon CloudWatch
- Created CPU utilization alarms with SNS email notifications
- Simulated high CPU usage to trigger alerts
- Demonstrated real-time infrastructure monitoring

## ⚖️ Application Load Balancer (ALB)
- Configured an Application Load Balancer to distribute traffic across multiple EC2 instances
- Created target groups and registered EC2 instances
- Tested traffic distribution across web servers
- Demonstrated high availability architecture

## 📈 Auto Scaling Group (ASG)
- Created an Auto Scaling Group to automatically launch and terminate EC2 instances
- Configured Launch Template using custom AMI
- Integrated Auto Scaling with ALB target groups
- Tested scaling behavior using CPU utilization stress testing

