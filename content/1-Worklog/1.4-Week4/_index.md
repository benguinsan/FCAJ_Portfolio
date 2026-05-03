---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

**Internship period (Week 4):** 30/03/2026 – 05/04/2026

### Week 4 objectives (assigned focus)

* **CloudWatch** for monitoring and observability (metrics, logs, alarms).
* First steps with **IaC** using **AWS CloudFormation**.
* Build a first **serverless** function with **AWS Lambda**.

### Weekly plan by day

| Day | Date | Activities | Reference |
| --- | --- | --- | --- |
| Mon | 30/03/2026 | **CloudWatch** metrics & dashboards; **Logs** groups/retention; **Alarms** + **SNS** notifications | [CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) |
| Tue | 31/03/2026 | **CloudFormation**: template structure (`Resources`, `Parameters`, `Outputs`); deploy a small stack | [CloudFormation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html) |
| Wed | 01/04/2026 | Stack updates & drift awareness; clean delete stack | [Drift detection](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-drift-detection-stack.html) |
| Thu | 02/04/2026 | **Lambda** console: handler, runtime, execution role; test invoke | [Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html) |
| Fri | 03/04/2026 | Lambda with environment variables; optional trigger (e.g. **API Gateway** HTTP API) read-through | [Lambda triggers](https://docs.aws.amazon.com/lambda/latest/dg/lambda-invocation.html) |

### What was achieved this week

* Set up basic **observability** with metrics, log groups, and actionable **alarms**.

* Deployed and updated a **CloudFormation** stack, respecting idempotent practices.

* Shipped a first **Lambda** function with a clear execution role and tested invocations.

* Captured templates and runbooks for reuse in the SpendWise / workshop track.
