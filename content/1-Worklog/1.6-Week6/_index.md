---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

Internship period (Week 6): 13/04/2026 – 19/04/2026

### Week 6 objectives:

* Continue hands-on practice and read documentation (continuing workshop/lab work from prior weeks).
* Learn and complete the Amazon Cognito lab (user pool, app client, sign-in flow).
* Implement user authentication for the project app with Cognito and Terraform, including a VPC interface endpoint for the cognito-idp service (DNS pattern com.amazonaws.<REGION>.cognito-idp) so private traffic does not go through a NAT Gateway (reducing NAT dependency and optimizing cost/egress).
* Build and trial hosting for the frontend (or a suitable full-stack setup) with AWS Amplify.

### Tasks for this week:

| Day | Tasks | Start date | Completion date | Reference |
| --- | --- | --- | --- | --- |
| 2 | - Continue hands-on work from the lab guide / in-progress labs.<br>- Read the Amazon Cognito overview (user pools vs identity pools; project use cases). | 13/04/2026 | 13/04/2026 | [Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) |
| 3 | - Cognito lab: create a user pool and app client; try the hosted UI or a basic token flow in a sandbox.<br>- Note callback URLs, scopes, and client secrets (if used). | 14/04/2026 | 14/04/2026 | [Hosted UI](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |
| 4 | - Terraform: define Cognito (pool, client) and related networking.<br>- Create a VPC interface endpoint for the service DNS pattern com.amazonaws.<REGION>.cognito-idp (replace REGION with your deployment Region code) in private subnets; update route tables / security groups to allow HTTPS to the endpoint; confirm apps/workers in the VPC call Cognito without needing Internet egress via NAT. | 15/04/2026 | 15/04/2026 | [VPC endpoints](https://docs.aws.amazon.com/vpc/latest/privatelink/interface-endpoints.html) |
| 5 | - Finish application authentication integration with Cognito (environment variables, JWKS, refresh tokens — per team architecture).<br>- Test sign-in and token retrieval in dev. | 16/04/2026 | 16/04/2026 | [Cognito app integration](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |
| 6 | - AWS Amplify: create an app, connect the Git repo, configure build branches; trial build & deploy hosting.<br>- Align with Cognito (domain / redirects if using Amplify Hosting with auth). | 17/04/2026 | 17/04/2026 | [Amplify Hosting](https://docs.aws.amazon.com/amplify/latest/userguide/welcome.html) |

### Week 6 outcomes:

* Continued hands-on practice and documentation study on the project schedule.

* Completed the basic Cognito lab and understood the authentication flow suited to the app.

* Deployed Cognito with Terraform and a cognito-idp VPC endpoint, allowing Cognito API calls from private networks without relying on a NAT Gateway, as the chosen optimization approach.

* Trialled Amplify Hosting (build/deploy) and recorded how it ties into the auth flow when configured.
