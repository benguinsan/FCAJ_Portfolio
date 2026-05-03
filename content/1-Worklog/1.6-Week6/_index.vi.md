---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

Thời gian thực tập (tuần 6): 13/04/2026 – 19/04/2026

### Mục tiêu tuần 6:

* Tiếp tục thực hành và đọc tài liệu (nối tiếp workshop / lab các tuần trước).
* Tìm hiểu và thực hành lab Amazon Cognito (user pool, app client, luồng đăng nhập).
* Triển khai xác thực người dùng cho ứng dụng đồ án bằng Cognito kết hợp Terraform, trong đó có VPC interface endpoint tới dịch vụ cognito-idp (DNS dạng com.amazonaws.<REGION>.cognito-idp) để luồng private không đi qua NAT Gateway (giảm phụ thuộc NAT và tối ưu chi phí/luồng egress).
* Xây dựng và thử nghiệm hosting frontend (hoặc full-stack phù hợp) qua AWS Amplify.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tiếp tục thực hành theo tài liệu / lab đang dở.<br>- Đọc tổng quan Amazon Cognito (User Pool vs Identity Pool; use case đồ án). | 13/04/2026 | 13/04/2026 | [Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) |
| 3 | - Lab Cognito: tạo User Pool, App client; thử Hosted UI hoặc luồng token cơ bản trên môi trường thử.<br>- Ghi chú callback URL, scope, bí mật client (nếu dùng). | 14/04/2026 | 14/04/2026 | [Hosted UI](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |
| 4 | - Terraform: định nghĩa Cognito (pool, client) và tài nguyên mạng liên quan.<br>- Tạo VPC Interface Endpoint tới DNS dịch vụ dạng com.amazonaws.<REGION>.cognito-idp (thay REGION bằng mã vùng triển khai) trong subnet private; cập nhật route table / security group cho phép HTTPS tới endpoint; xác nhận ứng dụng/worker trong VPC gọi Cognito không cần ra Internet qua NAT. | 15/04/2026 | 15/04/2026 | [VPC endpoints](https://docs.aws.amazon.com/vpc/latest/privatelink/interface-endpoints.html) |
| 5 | - Hoàn thiện tích hợp xác thực ứng dụng với Cognito (biến môi trường, JWKS, refresh token — theo kiến trúc nhóm).<br>- Kiểm thử đăng nhập / lấy token từ môi trường dev. | 16/04/2026 | 16/04/2026 | [Cognito app integration](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-app-integration.html) |
| 6 | - AWS Amplify: tạo app, kết nối repo (Git), cấu hình nhánh build; chạy thử build & deploy hosting.<br>- Đối chiếu với Cognito (domain / redirect nếu dùng Amplify Hosting + auth). | 17/04/2026 | 17/04/2026 | [Amplify Hosting](https://docs.aws.amazon.com/amplify/latest/userguide/welcome.html) |

### Kết quả đạt được tuần 6:

* Đã nối tiếp thực hành và đọc tài liệu theo tiến độ đồ án.

* Hoàn thành phần lab Cognito cơ bản và nắm luồng xác thực phù hợp ứng dụng.

* Đã triển khai Cognito bằng Terraform kèm VPC endpoint cognito-idp, cho phép gọi API Cognito từ mạng private không phụ thuộc NAT Gateway như hướng tối ưu đã chọn.

* Đã thử nghiệm Amplify Hosting (build/deploy) và ghi nhận bước liên hệ với luồng auth nếu có cấu hình.
