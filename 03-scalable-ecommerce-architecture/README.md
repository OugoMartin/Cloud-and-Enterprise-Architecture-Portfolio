# 03 — Scalable Cloud Architecture for E-Commerce

## Objective
Architect a resilient and cost-conscious e-commerce platform using cloud-native services.

## AWS Services
- Amazon EC2
- Auto Scaling
- Elastic Load Balancing
- Amazon RDS
- Amazon S3
- AWS Pricing Calculator (cost-efficiency analysis)

## Architecture Concept
```text
Users
  |
  v
Elastic Load Balancing
  |
  v
EC2 / Auto Scaling
  |
  +-----------> Amazon RDS
  |
  +-----------> Amazon S3
```

The design uses load balancing and automatic scaling to address traffic surges. RDS supports database operations, while S3 provides object storage.

## Architecture Goals
- Scalability during changing traffic demand
- Resilience through distributed application capacity
- Managed database operations
- Object storage separation
- Cost awareness

## Cost Consideration
The source portfolio states that a cost-efficiency analysis was performed with the AWS Pricing Calculator. It does not provide the original calculator inputs or numerical results, so no cost figures are asserted here.

## Portfolio Value
This case study demonstrates architecture thinking around scalability, availability, cloud service selection, and cost trade-offs.
