# Scalability Design

## Traffic Management
Elastic Load Balancing distributes incoming application traffic across compute resources.

## Elastic Compute
EC2 instances combined with Auto Scaling are used conceptually to increase or decrease application capacity in response to demand.

## Data Services
Amazon RDS is assigned database operations while Amazon S3 is assigned object storage, separating storage responsibilities from the compute tier.

## Design Trade-offs to Evaluate
- Performance requirements versus cost
- Minimum/maximum compute capacity
- Database capacity and availability requirements
- Storage growth
- Operational complexity

The source portfolio establishes these services and objectives but does not specify production sizing, thresholds, availability-zone topology, or measured performance results.
