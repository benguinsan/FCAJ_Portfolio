---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

Internship period (Week 7): 20/04/2026 – 26/04/2026

### Week 7 objectives:

* Continue hands-on practice and read documentation (continuing workshop/lab work from prior weeks).
* Understand how Amazon ECS works and which VPC interface endpoints support running tasks on private networks: pulling images from ECR, calling the ECS control plane API, and logging (per team architecture — typically endpoints for ecr.api and ecr.dkr in the Region; add ecs, CloudWatch Logs, and other services as the app requires).
* Build the main backend components of the project with Terraform: ALB, ECR, ECS (cluster, service, task definition), and monitoring (CloudWatch dashboards/alarms or Container Insights — as agreed with the team).
* End-to-end testing: docker push images to ECR, run the service on ECS Fargate, reach it via the ALB DNS name, and exercise sign-up/sign-in together with Cognito deployed in week 6.

### Tasks for this week:

| Day | Tasks | Start date | Completion date | Reference |
| --- | --- | --- | --- | --- |
| 2 | - Continue hands-on work from the lab guide / in-progress labs.<br>- Read the ECS overview (cluster, service, task, Fargate launch type); review VPC endpoint needs when tasks run in private subnets (ECR, ECS API, logging). | 20/04/2026 | 20/04/2026 | [ECS](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html) |
| 3 | - Terraform: create an ECR repository and lifecycle policy (if any); ECS cluster; basic task execution role / task role.<br>- Design or update security groups for the ALB and tasks. | 21/04/2026 | 21/04/2026 | [ECR](https://docs.aws.amazon.com/AmazonECR/latest/userguide/what-is-ecr.html) |
| 4 | - Terraform: ALB, target group, listener (HTTP/HTTPS per team); ECS service attached to the target group; task definition referencing the ECR image.<br>- Create VPC interface endpoints for required services (for example DNS names com.amazonaws.<REGION>.ecr.api and com.amazonaws.<REGION>.ecr.dkr — replace REGION with your Region code); configure route tables / security groups for HTTPS to the endpoints. | 22/04/2026 | 22/04/2026 | [VPC endpoints for ECR](https://docs.aws.amazon.com/AmazonECR/latest/userguide/vpc-endpoints.html) |
| 5 | - Add monitoring: CloudWatch log groups, metrics/alarms for ECS or the ALB (per architecture).<br>- Verify tasks pull images and register healthy on the target group. | 23/04/2026 | 23/04/2026 | [CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) |
| 6 | - Build an image locally, docker push to ECR; update the task revision / rolling deploy on Fargate.<br>- Test via the ALB DNS name: sign-up/sign-in flow with week-6 Cognito (redirects, environment variables, JWT — per the app). | 24/04/2026 | 24/04/2026 | [Fargate](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html) |

### Week 7 outcomes:

* Continued hands-on practice and documentation study on the project schedule.

* Understood the ECS-on-Fargate flow and how VPC endpoints support image pulls / task orchestration on private networks.

* Deployed ALB, ECR, ECS, and a baseline monitoring layer with Terraform for the project backend.

* Pushed images to ECR, ran tasks on Fargate, and tested access through the ALB together with Cognito authentication from the previous week.
