---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

**Internship period (Week 2):** 16/03/2026 – 22/03/2026

### Week 2 objectives (assigned focus)

* Learn and practice core **AWS networking**: **VPC**, **subnets**, **route tables**, **Security Groups**.
* Practice provisioning **EC2** instances and basic connectivity.

### Weekly plan by day

| Day | Date | Activities | Reference |
| --- | --- | --- | --- |
| Mon | 16/03/2026 | VPC fundamentals: CIDR, AZs, public vs private subnets; **Internet Gateway** | [VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) |
| Tue | 17/03/2026 | **Security Groups** vs **NACLs**; lab: rules for HTTP/SSH | [Security groups](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html) |
| Wed | 18/03/2026 | **EC2**: AMIs, instance types, key pairs, **EBS** volumes | [EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) |
| Thu | 19/03/2026 | Launch EC2 in a custom VPC; attach **Elastic IP** (where appropriate); **SSH** / **SSM Session Manager** | [Connect to Linux instance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstances.html) |
| Fri | 20/03/2026 | End-to-end mini lab: VPC + subnets + SG + EC2; tear-down checklist | [AWS Study Group — Cloud Journey](https://cloudjourney.awsstudygroup.com/) |

### What was achieved this week

* Designed a simple **VPC** layout with subnets and routing aligned to security best practices.

* Configured **Security Groups** / **NACLs** for controlled inbound/outbound traffic.

* Launched and accessed **EC2** instances; practiced **EBS** attach/detach and basic troubleshooting.

* Documented the lab topology for reuse in the group project and later workshops.
