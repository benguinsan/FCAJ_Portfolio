---
title: "Worklog Tuần 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Mục tiêu tuần 3:

* Hiểu cách hoạt động và triển khai ELB.
* Tìm hiểu và thực hành xây dựng Auto Scaling Group cho EC2 instance.
* Nắm được các thành phần cơ bản của dịch vụ giám sát CloudWatch.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Đọc tài liệu tổng quan ELB (ALB/NLB), kiến trúc và các thành phần chính (Listener, Target Group, Health Check).<br>- Thực hành tạo ALB cơ bản và gắn vào 2 EC2 instance để kiểm tra phân phối traffic. | 23/03/2026 | 23/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Tìm hiểu Auto Scaling Group: Launch Template, min/desired/max capacity, scaling policy.<br>- Thực hành tạo ASG cho EC2 và gắn ASG vào Target Group của ALB.<br>- Kiểm tra tự động thay thế instance khi instance lỗi. | 24/03/2026 | 24/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Cấu hình Scaling Policy (target tracking theo CPU) cho ASG.<br>- Thực hành giả lập tải để quan sát scale out/scale in.<br>- Ghi nhận kết quả thay đổi số lượng instance theo từng ngưỡng tải. | 25/03/2026 | 25/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Tìm hiểu CloudWatch cơ bản: Metrics, Logs, Alarms, Dashboard.<br>- Tạo dashboard theo dõi nhanh các chỉ số của ELB và ASG. | 26/03/2026 | 26/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Tổng hợp kiến trúc hoàn chỉnh ELB + ASG + CloudWatch.<br>- Chạy kiểm thử end-to-end: cân bằng tải, tự động mở rộng, giám sát và cảnh báo. | 27/03/2026 | 27/03/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 3:

* Triển khai thành công ALB với các EC2 target và kiểm tra phân phối tải.
* Xây dựng, cấu hình và kiểm thử Auto Scaling Group tích hợp với Target Group của ALB.
* Theo dõi được hành vi scale out/scale in theo chính sách target tracking CPU.
* Thiết lập dashboard CloudWatch và giám sát cơ bản.
* Hoàn tất kiểm thử end-to-end cho luồng cân bằng tải, tự động mở rộng và giám sát.
