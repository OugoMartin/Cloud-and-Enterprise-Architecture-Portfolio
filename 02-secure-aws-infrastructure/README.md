# 02 — Secure AWS Infrastructure Design

## Objective
Build and document a secure AWS network architecture with isolated database resources, controlled network access, encryption, and protected credential management.

## Hands-On AWS Lab
The **Configuring a Secure VPC & Encrypted RDS in AWS Free Tier** lab provides implementation evidence for this case study.

### Lab configuration
- VPC: `MySecureVPC` — `10.0.0.0/16`
- Public subnet: `10.0.1.0/24`
- Private subnet: `10.0.2.0/24`
- Internet Gateway connected to the public route
- Web Security Group: HTTP/HTTPS plus SSH restricted to the user's IP
- PostgreSQL RDS `db.t3.micro` in the private subnet
- RDS encryption enabled with AWS-managed KMS
- Database credentials stored as SSM Parameter Store `SecureString` values

## Lab Screenshot Evidence
The uploaded lab contains screenshots documenting:
1. Public subnet configuration
2. Private subnet configuration
3. Internet Gateway configuration
4. Security Group configuration
5. Encrypted RDS configuration
6. Secure VPC/RDS architecture

## Technologies and Controls
- Amazon VPC
- Amazon RDS
- AWS IAM
- AWS Systems Manager Parameter Store
- AWS KMS
- Security Groups
- Encryption at rest
- Network isolation
- Secure credential storage

## Key Design Challenge
The lab identifies subnet routing as a primary implementation challenge: internet access had to remain available to the public subnet while the database remained isolated in the private subnet.

## Security Principles Demonstrated
1. Network segmentation
2. Least exposure
3. Restricted administrative access
4. Database encryption
5. Private database placement
6. Protected credential management

## Portfolio Value
This project now contains documented hands-on evidence rather than only a conceptual architecture. It demonstrates practical AWS networking, database security, encryption, and secrets-management experience.

## Evidence Boundary
The lab supports the configurations listed above. The repository does not claim Terraform/CloudFormation automation or production deployment because those artifacts were not supplied.
