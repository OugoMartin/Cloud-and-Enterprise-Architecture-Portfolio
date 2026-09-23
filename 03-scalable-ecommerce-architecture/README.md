# 03 — AWS Web Application Deployment & Scalable E-Commerce Architecture

## Objective
Demonstrate hands-on AWS web-application deployment and connect the implementation to a scalable, resilient e-commerce architecture.

## Hands-On AWS Lab
The **Deploying a Web Application with AWS** lab integrates VPC, EC2, S3, RDS, and CloudWatch using AWS Free Tier resources.

### Implemented configuration
- VPC: `MyWebAppVPC` — `10.0.0.0/16`
- Public subnet: `10.0.1.0/24`
- Private subnet: `10.0.2.0/24`
- EC2: `t2.micro`, Amazon Linux 2
- Apache web server with a custom web page
- Security Group: SSH from the user's IP and HTTP on port 80
- S3 bucket for application static assets
- PostgreSQL RDS `db.t3.micro`, 20 GB gp2, placed in the private subnet
- CloudWatch monitoring for EC2 and RDS
- CloudWatch CPU alarm threshold: 70%

## Lab Screenshot Evidence
The uploaded presentation includes screenshots demonstrating:
1. VPC/network configuration
2. Running web application on EC2
3. S3 bucket and uploaded application file
4. RDS instance configuration
5. CloudWatch dashboard and alarms

## Architecture Concept
```text
Users
  |
  v
EC2 Web Application
  |
  +-----------> Amazon RDS (private subnet)
  |
  +-----------> Amazon S3

Monitoring: Amazon CloudWatch
```

The broader portfolio extends this implementation concept with Auto Scaling and Elastic Load Balancing for traffic surges.

## Architecture Goals
- Secure network separation
- Compute hosting
- Managed relational database
- Object/static storage
- Resource monitoring and alarms
- Scalability and resilience
- Cost awareness

## Cost Consideration
The broader architecture portfolio records AWS Pricing Calculator analysis, but the original calculator inputs and numerical results were not supplied. No cost figures are invented here.

## Portfolio Value
This case study now combines a documented hands-on AWS deployment with architecture-level scalability planning, giving recruiters evidence of both implementation and design thinking.
