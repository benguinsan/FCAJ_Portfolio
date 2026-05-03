---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

Internship period (Week 8): 27/04/2026 – 02/05/2026

### Week 8 objectives (closure week):

* Deploy Amazon RDS for PostgreSQL for the project system (subnets, security groups, baseline parameters, backups — per team architecture).
* Deploy Amazon CloudFront in front of static assets or the application origin (ALB/S3 origin — per design) to distribute traffic and reduce direct load on the ALB where applicable.
* Deploy AWS WAF on the ALB (or on CloudFront for edge WAF) to strengthen security (baseline rules, rate limits, logging — within demo scope).
* Finish deploying the full application to AWS (review environment variables, secrets, health checks, and the existing auth flow).
* Summarize internship outcomes and complete the report.

### Tasks for this week:

| Day | Tasks | Start date | Completion date | Reference |
| --- | --- | --- | --- | --- |
| 2 | - Terraform or team IaC: create a PostgreSQL RDS instance (engine version and class sized for the demo), DB subnet group, and security groups that only allow traffic from ECS/ALB as designed.<br>- Document the endpoint and the difference between admin DB users and application users. | 27/04/2026 | 27/04/2026 | [RDS PostgreSQL](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html) |
| 3 | - Test application connectivity to RDS; enable automated backups / minimum retention per team policy.<br>- Run migrations or initial schema work (if in scope this week). | 28/04/2026 | 28/04/2026 | [Connecting to RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_CommonTasks.Connect.html) |
| 4 | - Terraform: stand up CloudFront (distribution, origin, basic caching behavior, TLS certificate if using HTTPS).<br>- Validate headers/cookies the app needs behind the CDN. | 29/04/2026 | 29/04/2026 | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| 5 | - Attach AWS WAF to the ALB or to CloudFront (per architecture); configure a minimal managed/custom rule set; enable WAF logging if needed for the demo.<br>- Test allowed vs blocked requests. | 30/04/2026 | 30/04/2026 | [AWS WAF](https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html) |
| 6 | - Complete end-to-end deployment: ALB, ECS, RDS, CloudFront, WAF, Cognito, and other existing components; ship a stable build to the agreed environment.<br>- Review health checks, key alarms, and deployment README. | 01/05/2026 | 01/05/2026 | [Well-Architected](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html) |
| 7 | - Write the internship report (worklog, architecture, outcomes, lessons learned); rehearse the demo.<br>- Clean-up / handover: credentials, resource tags, and a checklist to delete or keep environments per mentor guidance. | 02/05/2026 | 02/05/2026 | - |

### Week 8 outcomes:

* Delivered PostgreSQL on RDS for the system and connected the application per team design.

* Delivered CloudFront and integrated it with the application traffic pattern (appropriate origin).

* Deployed WAF on the ALB or CloudFront, adding a basic protection layer against abusive traffic.

* Completed full-application deployment to AWS within the final demo scope.

* Finished the internship report and handed over documentation and environment status using the checklist.
