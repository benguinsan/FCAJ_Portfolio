---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Week 3 objectives:

* Understand how **Elastic Load Balancing (ELB)** works and how to deploy it.
* Learn and practise building an **Auto Scaling Group** for EC2 instances.
* Learn the basics of **Amazon CloudWatch** for monitoring.

### Tasks for this week:

| Day | Tasks | Start date | Completion date | Reference |
| --- | --- | --- | --- | --- |
| 2 | - Read ELB overview (ALB/NLB), architecture, and key components (listener, target group, health checks).<br>- Practise creating a basic ALB attached to two EC2 instances to verify traffic distribution. | 23/03/2026 | 23/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Learn Auto Scaling groups: launch template, min/desired/max capacity, scaling policies.<br>- Practise creating an ASG for EC2 and attaching it to the ALB target group.<br>- Verify automatic instance replacement when an instance fails. | 24/03/2026 | 24/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Configure a CPU **target tracking** scaling policy for the ASG.<br>- Simulate load to observe scale-out and scale-in.<br>- Record how instance counts change at different load levels. | 25/03/2026 | 25/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Learn CloudWatch basics: metrics, logs, alarms, dashboards.<br>- Build a quick dashboard for ELB and ASG metrics. | 26/03/2026 | 26/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Consolidate the full **ELB + ASG + CloudWatch** architecture.<br>- Run an end-to-end test: load balancing, autoscaling, monitoring, and alarms. | 27/03/2026 | 27/03/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Week 3 outcomes:

* Deployed an ALB with EC2 targets and verified load distribution.

* Built, configured, and tested an ASG integrated with the ALB target group.

* Observed scale-out/scale-in behaviour under a CPU target tracking policy.

* Set up a CloudWatch dashboard and basic monitoring.

* Completed end-to-end testing for load balancing, autoscaling, and monitoring.
