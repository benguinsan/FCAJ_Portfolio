---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
### Week 2 objectives:

* Study and practise the AWS **Compute** family: **EC2, AMI, EBS, Auto Scaling, ALB**.
* Learn the storage family: **S3** and **AWS Storage Gateway**.
* Practise deploying and hosting a **static website on S3**.

### Tasks for this week:

| Day | Tasks | Start date | Completion date | Reference |
| --- | --- | --- | --- | --- |
| 2 | - Read Amazon EC2 documentation; learn instance types and cost optimisation (Spot, Reserved, Savings Plans).<br>- Practise basic EC2 provisioning.<br>- Understand durable storage with EBS.<br>- Practise backup/cloning with AMIs and snapshots. | 16/03/2026 | 16/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Lab: deploy Node.js on EC2.<br>- Create a VPC, configure security groups, launch EC2.<br>- Connect securely over SSH. | 17/03/2026 | 17/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Continue Node.js on EC2.<br>- Install and configure LAMP.<br>- Install Node.js on Linux and finish deploying the application. | 18/03/2026 | 18/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Learn AWS Storage Gateway and Amazon S3.<br>- Practise creating and configuring an S3 bucket and working with objects.<br>- Practise cross-region replication for HA. | 19/03/2026 | 19/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Practise static website hosting on S3.<br>- Use CloudFront.<br>- Configure CORS and OAC to protect access to the S3 bucket.<br>- Learn bucket versioning. | 20/03/2026 | 20/03/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Week 2 outcomes:

* Completed the hands-on path from EC2 infrastructure to deploying Node.js on AWS.

* Understood core compute building blocks: AMI, EBS, instance types, and basic scaling/load balancing.

* Completed S3 exercises: bucket creation, object operations, static site hosting, and basic CloudFront integration.

* Learned more about data protection and availability: snapshots, replication, OAC, CORS, and versioning.

### Challenges and how they were addressed:

* **Challenge:** When deploying Node.js, the EC2 instance sometimes slowed or stalled during dependency installation because of limited RAM on a small instance.

* **Approach (as adopted):** Add **swap** on EBS, enable it, and tune **swappiness** to reduce memory pressure during install/build.
