---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---
### Week 4 objectives:

* Learn and practise deploying **Amazon RDS** (SQL model).
* Get started with **IaC on AWS using CloudFormation** (lab-based exercises).
* **Define the project topic** and **select AWS services** suited to the application.

### Tasks for this week:

| Day | Tasks | Start date | Completion date | Reference |
| --- | --- | --- | --- | --- |
| 2 | - Read the Amazon RDS for MySQL overview: architecture, instance class, storage, and security groups.<br>- Practise creating RDS MySQL per the course lab.<br>- Launch EC2 in the appropriate VPC/subnet to prepare for RDS connectivity. | 30/03/2026 | 30/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Configure connectivity from EC2 to RDS (security group inbound/outbound, endpoint, port 3306).<br>- Verify database connectivity from EC2 using a MySQL client.<br>- Create sample schema/tables for CRUD testing. | 31/03/2026 | 31/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Install Node.js on EC2 and configure environment variables for RDS.<br>- Deploy a Node.js CRUD app connected to RDS MySQL.<br>- Exercise Create/Read/Update/Delete flows and record results. | 01/04/2026 | 01/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Learn CloudFormation following the course lab step by step.<br>- Deploy the stack per lab instructions.<br>- Watch the **Events** tab and troubleshoot using the lab guide. | 02/04/2026 | 02/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Define the project topic: **personal expense management app** (scope, users, main data flows).<br>- Choose an initial AWS service set (frontend/hosting, API, database, auth, file storage, monitoring) balancing **realism** and **cost optimisation**. | 03/04/2026 | 03/04/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Week 4 outcomes:

* Deployed **RDS MySQL** per the lab and launched suitable **EC2** for database connectivity.

* Completed **EC2 → RDS** connectivity checks and prepared **sample schema/tables** for CRUD tests.

* Ran a **Node.js CRUD** app on EC2 against RDS and verified basic **Create/Read/Update/Delete** operations.

* Practised **CloudFormation** per the lab, monitored **Events**, and fixed issues using the guide.

* Clarified the **project topic** and an initial **AWS service** set, balancing realism and cost.
