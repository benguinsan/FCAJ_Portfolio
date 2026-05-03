---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

**Internship period (Week 6):** 13/04/2026 – 19/04/2026

### Week 6 objectives (assigned focus)

* User authentication with **Amazon Cognito** (user pools, app clients, hosted UI concepts).
* Contribute to group project infrastructure: **VPC** & **Security Groups** baseline.
* Align **Cognito** with the application’s sign-in / token flow.

### Weekly plan by day

| Day | Date | Activities | Reference |
| --- | --- | --- | --- |
| Mon | 13/04/2026 | **Cognito** user pools; password/MFA policies; app client settings | [Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) |
| Tue | 14/04/2026 | Hosted UI & OAuth/OIDC flows (read + diagram); test tokens in sandbox | [Hosted UI](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |
| Wed | 15/04/2026 | Group project: review **VPC** diagram (subnets, IGW, NAT, endpoints) | Team design doc |
| Thu | 16/04/2026 | Implement / refine **Security Groups** for ALB, ECS tasks, RDS in repo (`terraform`/`cdk`) | Repo + mentor review |
| Fri | 17/04/2026 | Wire **Cognito** client IDs & callback URLs to dev environment; document secrets handling | [Cognito app integration](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |

### What was achieved this week

* Configured a **Cognito** user pool suitable for dev/testing and understood token lifecycles.

* Contributed **networking** changes (VPC + **SG** rules) reviewed with the team.

* Produced integration notes for frontend/backend teams on **auth** configuration.
