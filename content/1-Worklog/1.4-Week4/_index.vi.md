---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

**Thời gian thực tập (tuần 4):** 30/03/2026 – 05/04/2026

### Mục tiêu tuần 4 (theo nội dung giao tại đơn vị)

* **CloudWatch** — monitoring và observability (metric, log, alarm).
* Làm quen **IaC** qua **AWS CloudFormation**.
* Xây dựng hàm **serverless** với **AWS Lambda**.

### Kế hoạch công việc theo ngày

| Thứ | Ngày | Nội dung công việc | Tài liệu |
| --- | --- | --- | --- |
| 2 | 30/03/2026 | **CloudWatch** metric & dashboard; **Logs**; **Alarm** + **SNS** | [CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) |
| 3 | 31/03/2026 | **CloudFormation**: template (`Resources`, `Parameters`, `Outputs`); deploy stack nhỏ | [CloudFormation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html) |
| 4 | 01/04/2026 | Cập nhật stack; nhận biết drift; xóa stack gọn | [Drift](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-drift-detection-stack.html) |
| 5 | 02/04/2026 | **Lambda**: handler, runtime, execution role; test invoke | [Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html) |
| 6 | 03/04/2026 | Biến môi trường Lambda; đọc/ghi nhận trigger (ví dụ **API Gateway** HTTP API) | [Lambda triggers](https://docs.aws.amazon.com/lambda/latest/dg/lambda-invocation.html) |

### Kết quả đạt được trong tuần

* Thiết lập **quan sát** cơ bản: metric, log group, **alarm** có hành động.

* Triển khai và cập nhật stack **CloudFormation** theo hướng idempotent.

* Hoàn thành hàm **Lambda** đầu tiên với role rõ ràng và kiểm thử invoke.

* Lưu template/runbook phục vụ chuỗi SpendWise / workshop.
