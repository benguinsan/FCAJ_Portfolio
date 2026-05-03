---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

Thời gian thực tập (tuần 7): 20/04/2026 – 26/04/2026

### Mục tiêu tuần 7:

* Tiếp tục thực hành và đọc tài liệu (nối tiếp workshop / lab các tuần trước).
* Nắm cách hoạt động của Amazon ECS và các VPC interface endpoint phục vụ triển khai task trên mạng private: kéo image từ ECR, gọi API điều phối ECS, ghi log (theo kiến trúc nhóm — thường cần endpoint tới ecr.api, ecr.dkr trong region; bổ sung ecs, CloudWatch Logs và tài nguyên khác nếu app yêu cầu).
* Xây dựng các thành phần backend chính của đồ án bằng Terraform: ALB, ECR, ECS (cluster, service, task definition) và giám sát (CloudWatch dashboard / alarm hoặc Container Insights — theo thống nhất nhóm).
* Kiểm thử end-to-end: docker push image lên ECR, chạy service trên ECS Fargate, truy cập qua DNS của ALB và thử đăng ký / đăng nhập kết hợp Cognito đã triển khai ở tuần 6.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tiếp tục thực hành theo tài liệu / lab đang dở.<br>- Đọc tổng quan ECS (cluster, service, task, launch type Fargate); xem lại yêu cầu VPC endpoint khi task chạy trong subnet private (ECR, ECS API, log). | 20/04/2026 | 20/04/2026 | [ECS](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html) |
| 3 | - Terraform: khởi tạo ECR repository, lifecycle policy (nếu có); cluster ECS; task execution role / task role cơ bản.<br>- Thiết kế hoặc cập nhật security group cho ALB và task. | 21/04/2026 | 21/04/2026 | [ECR](https://docs.aws.amazon.com/AmazonECR/latest/userguide/what-is-ecr.html) |
| 4 | - Terraform: ALB, target group, listener (HTTP/HTTPS theo nhóm); ECS service nối target group; task definition trỏ image ECR.<br>- Tạo VPC interface endpoint tới các dịch vụ cần thiết (ví dụ DNS dạng com.amazonaws.<REGION>.ecr.api, com.amazonaws.<REGION>.ecr.dkr — thay REGION bằng mã vùng); cấu hình route table / security group cho HTTPS tới endpoint. | 22/04/2026 | 22/04/2026 | [VPC endpoints cho ECR](https://docs.aws.amazon.com/AmazonECR/latest/userguide/vpc-endpoints.html) |
| 5 | - Bổ sung giám sát: log group CloudWatch, metric / alarm liên quan ECS hoặc ALB (theo kiến trúc).<br>- Kiểm tra task pull image và healthy trên target group. | 23/04/2026 | 23/04/2026 | [CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) |
| 6 | - Build image cục bộ, docker push lên ECR; cập nhật revision task / rolling deploy Fargate.<br>- Kiểm thử qua DNS của ALB: luồng đăng ký / đăng nhập với Cognito tuần 6 (redirect, biến môi trường, JWT — theo app). | 24/04/2026 | 24/04/2026 | [Fargate](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html) |

### Kết quả đạt được tuần 7:

* Đã nối tiếp thực hành và đọc tài liệu theo tiến độ đồ án.

* Nắm luồng ECS trên Fargate và vai trò các VPC endpoint phục vụ pull image / điều phối task trong mạng private.

* Đã triển khai bằng Terraform các thành phần ALB, ECR, ECS và lớp giám sát cơ bản theo hướng backend đồ án.

* Đã đẩy image lên ECR, chạy task trên Fargate và kiểm thử truy cập qua ALB kết hợp xác thực Cognito từ tuần trước.
