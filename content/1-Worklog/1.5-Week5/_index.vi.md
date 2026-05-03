---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

**Thời gian thực tập (tuần 5):** 06/04/2026 – 12/04/2026

### Mục tiêu tuần 5 (theo nội dung giao tại đơn vị)

* Thực hành **Workshop mạng trên AWS** (theo lab đơn vị).
* Phân phối nội dung qua **CloudFront**.
* Tìm hiểu **AWS CDK** (cấu trúc project, `cdk synth`, `cdk deploy`).

### Kế hoạch công việc theo ngày

| Thứ | Ngày | Nội dung công việc | Tài liệu |
| --- | --- | --- | --- |
| 2 | 06/04/2026 | Workshop: ôn VPC/subnet/routing + bài tập mạng có hướng dẫn | Tài liệu workshop / mentor |
| 3 | 07/04/2026 | Workshop: cân bằng tải & mô hình TLS (lý thuyết + lab) | [ELB](https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/introduction.html) |
| 4 | 08/04/2026 | Lab **CloudFront**: distribution, origin **S3** hoặc **ALB**, cache policy | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| 5 | 09/04/2026 | Cài **AWS CDK**; `cdk init`; stack **bootstrap**; construct đầu tiên | [CDK](https://docs.aws.amazon.com/cdk/v2/guide/home.html) |
| 6 | 10/04/2026 | CDK: `synth` & deploy stack nhỏ; ghi chú tham số & teardown | [CDK Workshop](https://cdkworkshop.com/) |

### Kết quả đạt được trong tuần

* Hoàn thành phần workshop **mạng** và liên hệ với kiến trúc nhóm.

* Cấu hình **CloudFront** với origin và hành vi cache được ghi lại.

* Khởi tạo ứng dụng **CDK** và deploy stack tối thiểu lên môi trường dev.

* Thống nhất quy ước đặt tên, tag, môi trường với nhóm **IaC**.
