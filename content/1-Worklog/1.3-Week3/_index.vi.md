---
title: "Worklog Tuần 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

**Thời gian thực tập (tuần 3):** 23/03/2026 – 29/03/2026

### Mục tiêu tuần 3 (theo nội dung giao tại đơn vị)

* Dịch vụ lưu trữ **S3** và phân phối nội dung với **CloudFront**.
* Dịch vụ quản trị CSDL **RDS**.
* Tìm hiểu **Auto Scaling Group** (khả năng mở rộng và sẵn sàng).

### Kế hoạch công việc theo ngày

| Thứ | Ngày | Nội dung công việc | Tài liệu |
| --- | --- | --- | --- |
| 2 | 23/03/2026 | **S3**: bucket, object, versioning, mã hóa, bucket policy | [S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) |
| 3 | 24/03/2026 | **CloudFront**: distribution, origin (S3/ALB), behaviour, invalidate cache cơ bản | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| 4 | 25/03/2026 | **RDS**: engine, subnet group, parameter group; tạo DB dev nhỏ | [RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) |
| 5 | 26/03/2026 | Kết nối **RDS** từ VPC ứng dụng; backup & snapshot | [RDS backups](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_CommonTasks.BackupRestore.html) |
| 6 | 27/03/2026 | **Auto Scaling Group** + **Launch Template**: desired/min/max; health check | [Auto Scaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html) |

### Kết quả đạt được trong tuần

* Thao tác **S3** ổn cho tài tĩnh và quyền truy cập theo policy.

* Thử nghiệm **CloudFront** phía trước origin **S3**.

* Triển khai **RDS** trong private subnet với cấu hình hợp lý và ghi lại bước kết nối.

* Hiểu vai trò **ASG** duy trì capacity trên nhiều AZ.
