# Cost Analysis Framework

The original project used the **AWS Pricing Calculator** for cost-efficiency analysis. Numerical assumptions/results were not included in the supplied portfolio, so this document records a reproducible framework rather than invented figures.

| Component | Inputs to Document |
|---|---|
| EC2 | Instance type, count, utilization assumptions, runtime |
| Load Balancing | Traffic/load assumptions |
| RDS | Engine, instance class, storage, availability configuration |
| S3 | Storage volume, request patterns, transfer assumptions |
| Scaling | Baseline and peak capacity assumptions |

A completed assessment should retain the date, region, architecture assumptions, workload assumptions, calculator estimate, and major cost drivers.
