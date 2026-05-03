---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

**Internship period (Week 5):** 06/04/2026 – 12/04/2026

### Week 5 objectives (assigned focus)

* Hands-on **AWS networking workshop** content (per company lab track).
* Distribute content via **CloudFront** (CDN behaviours, origins).
* Introduction to **AWS CDK** (project layout, `cdk synth`, `cdk deploy`).

### Weekly plan by day

| Day | Date | Activities | Reference |
| --- | --- | --- | --- |
| Mon | 06/04/2026 | Workshop: VPC / subnets / routing recap + guided network exercises | Workshop materials / mentor |
| Tue | 07/04/2026 | Workshop: load balancing & TLS termination patterns (concept + lab) | [ELB](https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/introduction.html) |
| Wed | 08/04/2026 | **CloudFront** lab: create distribution, attach **S3** or **ALB** origin, cache policy | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| Thu | 09/04/2026 | **AWS CDK** setup: Node/Java runtime; `cdk init`; **bootstrap** stack; first construct | [CDK](https://docs.aws.amazon.com/cdk/v2/guide/home.html) |
| Fri | 10/04/2026 | CDK: synthesize & deploy a small stack; document parameters & teardown | [CDK Workshop](https://cdkworkshop.com/) |

### What was achieved this week

* Completed targeted **network workshop** tasks and mapped them to the group architecture.

* Delivered static or API traffic through **CloudFront** with documented origin settings.

* Bootstrapped a **CDK** app and deployed a minimal stack to a dev account.

* Linked CDK outputs to the team’s **IaC** conventions (naming, tags, environments).
