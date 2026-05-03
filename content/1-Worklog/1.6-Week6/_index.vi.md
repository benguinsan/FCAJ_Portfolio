---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

**Thời gian thực tập (tuần 6):** 13/04/2026 – 19/04/2026

### Mục tiêu tuần 6 (theo nội dung giao tại đơn vị)

* Xác thực người dùng với **AWS Cognito**.
* Xây dựng phần hạ tầng đồ án nhóm: **VPC** — **Security Group** (networking).
* Tích hợp **Cognito** với luồng đăng nhập / token ứng dụng.

### Kế hoạch công việc theo ngày

| Thứ | Ngày | Nội dung công việc | Tài liệu |
| --- | --- | --- | --- |
| 2 | 13/04/2026 | **Cognito** user pool; chính sách mật khẩu/MFA; cấu hình app client | [Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) |
| 3 | 14/04/2026 | Hosted UI & luồng OAuth/OIDC (đọc + vẽ sơ đồ); thử token trên sandbox | [Hosted UI](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |
| 4 | 15/04/2026 | Đồ án nhóm: rà soát sơ đồ **VPC** (subnet, IGW, NAT, endpoint) | Tài liệu thiết kế nhóm |
| 5 | 16/04/2026 | Triển khai / chỉnh **Security Group** cho ALB, ECS, RDS trong repo | Repo + review mentor |
| 6 | 17/04/2026 | Gắn client ID & callback **Cognito** vào môi trường dev; ghi chú bảo mật bí mật | [Cognito app integration](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |

### Kết quả đạt được trong tuần

* Cấu hình **Cognito** phục vụ dev/test và nắm vòng đời token.

* Đóng góp thay đổi **mạng** (VPC + **SG**) được nhóm review.

* Chuẩn bị tài liệu tích hợp cho frontend/backend về **xác thực**.
