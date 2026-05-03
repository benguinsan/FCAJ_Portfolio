---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

**Internship period (Week 3):** 23/03/2026 – 29/03/2026

### Week 3 objectives (assigned focus)

* **S3** storage patterns and static content delivery with **CloudFront**.
* **RDS** fundamentals for managed relational databases.
* Introduction to **Auto Scaling Groups** (capacity and availability).

### Weekly plan by day

| Day | Date | Activities | Reference |
| --- | --- | --- | --- |
| Mon | 23/03/2026 | **S3** buckets, objects, versioning, encryption options, bucket policies | [S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) |
| Tue | 24/03/2026 | **CloudFront** distributions: origins (S3/ALB), behaviours, cache invalidation basics | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| Wed | 25/03/2026 | **RDS** engines, subnet groups, parameter groups; create a small dev database | [RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) |
| Thu | 26/03/2026 | **RDS** connectivity from app VPC; backups & snapshots overview | [RDS backups](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_CommonTasks.BackupRestore.html) |
| Fri | 27/03/2026 | **Auto Scaling Groups** + **Launch Template**: desired/min/max; health checks | [Auto Scaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html) |

### What was achieved this week

* Built confidence with **S3** for static assets and policy-driven access.

* Sketched and tested a **CloudFront** distribution in front of an **S3** origin.

* Provisioned **RDS** in private subnets with sensible defaults and documented connection steps.

* Understood how **ASG** maintains capacity across AZs for resilient web tiers.
