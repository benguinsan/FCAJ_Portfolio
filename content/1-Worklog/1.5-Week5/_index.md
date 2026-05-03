---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

**Internship period (Week 5):** 06/04/2026 – 12/04/2026

### Week 5 objectives:

* Continue the **workshop** hands-on exercises following the course materials.
* Start the **architecture diagram** for the **personal expense management** project using **draw.io**.
* **Hands-on Amazon CloudFront lab** (content delivery / CDN).
* Begin **VPC and subnet** infrastructure for the project with **Terraform**.
* **Expected cost estimate** (per month or by traffic scenario) for **AWS services** planned for the app (cross-checked with the architecture diagram).

### Tasks for this week:

| Day | Tasks | Start date | Completion date | Reference |
| --- | --- | --- | --- | --- |
| 2 | - Continue the workshop from the lab guide (in-progress modules).<br>- Capture items to reflect in the architecture diagram. | 06/04/2026 | 06/04/2026 | Workshop materials |
| 3 | - Set up **draw.io** (desktop or web).<br>- Draft the diagram: users, frontend, API, database, main data flows for the personal expense app.<br>- Save the diagram using the team naming/version convention. | 07/04/2026 | 07/04/2026 | [draw.io](https://www.drawio.com/) |
| 4 | - **CloudFront lab:** create a distribution, origin (e.g. **S3** or **ALB**), behaviours, basic cache policy.<br>- Record the endpoint URL and verification steps. | 08/04/2026 | 08/04/2026 | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| 5 | - **Terraform:** initialise a module or stack for **VPC** (CIDR, AZs, public/private **subnets**).<br>- Run terraform fmt, validate, and plan in a dev environment.<br>- Align the draw.io diagram with resources defined in code. | 09/04/2026 | 09/04/2026 | [Terraform](https://developer.hashicorp.com/terraform) |
| 6 | - Finalise a minimal VPC/subnet baseline for the project; update README or code comments.<br>- **Expected cost estimate:** list services from the diagram (VPC, compute, database, S3, CloudFront, auth, monitoring, …); use an **assumptions table** and/or **Cost Explorer** (if your account or trial access allows) to estimate **USD/month** with clear assumptions (region, instance types, storage, requests).<br>- Review spend from experiments; tear down anything unnecessary (if applicable). | 10/04/2026 | 10/04/2026 | [Cost Explorer](https://docs.aws.amazon.com/cost-management/latest/userguide/ce-what-is.html) |

### Week 5 outcomes:

* Continued the workshop on schedule with the materials and clarified what still needs to move into the architecture view.

* Produced an initial **draw.io architecture** draft for the personal expense topic, aligned with the team.

* Completed the **CloudFront** hands-on lab (distribution, origin, access verification).

* Started **Terraform** for **VPC and subnets** for the project.

* Produced **notes or a table with expected cost estimates** for planned services (with assumptions and where prices were checked) to compare options and control lab spend.
