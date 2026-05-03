---
title: "Worklog Tuần 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
### Mục tiêu tuần 2:

* Đọc tài liệu và thực hành nhóm dịch vụ Compute của AWS: **EC2, AMI, EBS, Auto Scaling, ALB**.
* Tìm hiểu nhóm dịch vụ lưu trữ: **S3** và **AWS Storage Gateway**.
* Thực hành triển khai và hosting **website tĩnh trên S3**.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Đọc tài liệu Amazon EC2, tìm hiểu các loại instance và chiến lược tối ưu chi phí (Spot, Reserved, Savings Plans).<br>- Thực hành khởi tạo EC2 cơ bản.<br>- Hiểu lưu trữ bền vững qua EBS.<br>- Thực hành sao lưu/nhân bản bằng AMI và Snapshot. | 16/03/2026 | 16/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Thực hành lab triển khai Node.js trên EC2.<br>- Tạo VPC, cấu hình Security Group, khởi tạo EC2.<br>- Kết nối an toàn qua SSH. | 17/03/2026 | 17/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Tiếp tục triển khai Node.js trên EC2.<br>- Cài đặt và cấu hình LAMP.<br>- Cài Node.js trên Linux, hoàn thiện deploy ứng dụng. | 18/03/2026 | 18/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Tìm hiểu AWS Storage Gateway và Amazon S3.<br>- Thực hành tạo và cấu hình S3 bucket, thao tác object.<br>- Thực hành Cross-Region Replication để đảm bảo HA. | 19/03/2026 | 19/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Thực hành hosting web tĩnh trên S3.<br>- Ứng dụng CloudFront.<br>- Cấu hình CORS và OAC để bảo vệ truy cập S3 bucket.<br>- Tìm hiểu Bucket Versioning. | 20/03/2026 | 20/03/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 2:

* Hoàn thành luồng thực hành từ dựng hạ tầng EC2 đến triển khai Node.js lên trên hạ tầng AWS Cloud
* Nắm được các thành phần Compute cốt lõi: AMI, EBS, instance types và kiến thức cơ bản về scaling/load balancing.
* Hoàn thành thực hành S3: tạo bucket, thao tác object, hosting website tĩnh và tích hợp CloudFront cơ bản.
* Hiểu thêm về bảo vệ dữ liệu và tính sẵn sàng: Snapshot, replication, OAC, CORS và versioning.

### Khó khăn gặp phải và hướng xử lý:

* **Khó khăn:** Khi deploy Node.js, EC2 có lúc bị chậm/treo trong bước cài dependency do RAM hạn chế trên instance nhỏ.
* **Ý tưởng/Hướng xử lý (giữ nguyên):** Bổ sung **swap** trên EBS, kích hoạt và tinh chỉnh swappiness để giảm áp lực bộ nhớ trong lúc install/build.
