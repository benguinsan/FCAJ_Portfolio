---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

Thời gian thực tập (tuần 8): 27/04/2026 – 02/05/2026

### Mục tiêu tuần 8 (tuần kết thúc):

* Triển khai Amazon RDS for PostgreSQL cho hệ thống đồ án (subnet, security group, tham số cơ bản, backup — theo kiến trúc nhóm).
* Triển khai Amazon CloudFront phía trước nội dung tĩnh hoặc gốc ứng dụng (origin ALB/S3 — theo thiết kế) để phân phối và giảm tải trực tiếp lên ALB nếu có.
* Triển khai AWS WAF gắn với ALB (hoặc với CloudFront nếu WAF ở edge) để tăng cường bảo mật (rule cơ bản, rate limit, log — theo phạm vi demo).
* Hoàn thiện deploy toàn bộ ứng dụng lên môi trường AWS (rà soát biến môi trường, secret, health check, luồng auth đã có).
* Tổng hợp kết quả thực tập và hoàn thiện báo cáo

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Terraform hoặc IaC nhóm: tạo RDS PostgreSQL (phiên bản engine, kích thước instance phù hợp demo), subnet group, security group chỉ cho phép nguồn từ ECS/ALB theo thiết kế.<br>- Ghi chú endpoint, user quản trị CSDL vs user ứng dụng. | 27/04/2026 | 27/04/2026 | [RDS PostgreSQL](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html) |
| 3 | - Kiểm thử kết nối ứng dụng tới RDS; bật backup tự động / retention tối thiểu theo chính sách nhóm.<br>- Migration hoặc schema khởi tạo (nếu có trong phạm vi tuần). | 28/04/2026 | 28/04/2026 | [Kết nối RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_CommonTasks.Connect.html) |
| 4 | - Terraform: phân phối CloudFront (distribution, origin, hành vi cache cơ bản, certificate nếu HTTPS).<br>- Kiểm tra header / cookie cần thiết cho ứng dụng sau CDN. | 29/04/2026 | 29/04/2026 | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| 5 | - Gắn AWS WAF với ALB hoặc với CloudFront (theo kiến trúc); cấu hình tập rule mặc định / custom tối thiểu; bật logging WAF nếu cần demo.<br>- Kiểm thử request hợp lệ / bị chặn. | 30/04/2026 | 30/04/2026 | [AWS WAF](https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html) |
| 6 | - Hoàn thiện triển khai end-to-end: ALB, ECS, RDS, CloudFront, WAF, Cognito và các thành phần đã có; deploy bản ổn định lên môi trường thống nhất.<br>- Rà health check, alarm chính, README triển khai. | 01/05/2026 | 01/05/2026 | [Well-Architected](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html) |
| 7 | - Soạn báo cáo thực tập (worklog, kiến trúc, kết quả, rút kinh nghiệm); diễn tập demo.<br>- Dọn dẹp / bàn giao: credential, tag tài nguyên, checklist xóa hoặc giữ môi trường theo mentor. | 02/05/2026 | 02/05/2026 | Repo / mẫu báo cáo |

### Kết quả đạt được tuần 8:

* Đã triển khai RDS PostgreSQL phục vụ hệ thống và kết nối ứng dụng theo thiết kế nhóm.

* Đã triển khai CloudFront và tích hợp với luồng truy cập ứng dụng (origin phù hợp).

* Đã triển khai WAF gắn với ALB hoặc CloudFront, tăng cường lớp bảo vệ trước traffic độc hại cơ bản.

* Đã hoàn thiện deploy toàn bộ ứng dụng lên môi trường AWS trong phạm vi demo cuối kỳ.

* Đã tổng hợp và hoàn thiện báo cáo thực tập; bàn giao tài liệu và trạng thái môi trường theo checklist.
