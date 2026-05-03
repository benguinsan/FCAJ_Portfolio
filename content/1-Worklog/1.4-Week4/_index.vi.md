---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu tuần 4:

* Tìm hiểu và thực hành triển khai dịch vụ **Amazon RDS** (mô hình SQL).
* Bước đầu làm quen **IaC trên AWS với CloudFormation** (thực hành theo lab tài liệu).
* **Xác định đề tài dự án** và **lựa chọn các dịch vụ AWS** phù hợp cho ứng dụng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Đọc tài liệu tổng quan Amazon RDS for MySQL (mô hình SQL): kiến trúc, instance class, storage, và security group.<br>- Thực hành tạo RDS MySQL theo lab trên tài liệu.<br>- Khởi tạo EC2 trong cùng VPC/subnet phù hợp để chuẩn bị kết nối vào RDS. | 30/03/2026 | 30/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Cấu hình kết nối từ EC2 tới RDS (security group inbound/outbound, endpoint, port 3306).<br>- Kiểm tra kết nối database từ EC2 bằng MySQL client.<br>- Khởi tạo schema/table mẫu phục vụ test CRUD. | 31/03/2026 | 31/03/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Cài đặt môi trường Node.js trên EC2 và cấu hình biến môi trường kết nối RDS.<br>- Triển khai ứng dụng Node.js CRUD kết nối tới RDS MySQL.<br>- Chạy thử các chức năng Create/Read/Update/Delete và ghi nhận kết quả. | 01/04/2026 | 01/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Làm quen CloudFormation theo đúng lab trong tài liệu (thực hành bám sát hướng dẫn).<br>- Triển khai stack theo từng bước trong lab.<br>- Theo dõi tab Events, xử lý lỗi theo phần troubleshooting của tài liệu. | 02/04/2026 | 02/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Xác định đề tài dự án: **ứng dụng quản lý chi tiêu cá nhân** (phạm vi chức năng, đối tượng người dùng, luồng dữ liệu chính).<br>- Lựa chọn bộ dịch vụ AWS phù hợp (frontend/hosting, API, database, auth, lưu trữ file, giám sát) theo tiêu chí **gần thực tế** nhưng **tối ưu chi phí**. | 03/04/2026 | 03/04/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 4:

* Triển khai được **RDS MySQL** theo lab và khởi tạo **EC2** phù hợp để chuẩn bị kết nối database.
* Hoàn tất kiểm tra **kết nối EC2 → RDS** và chuẩn bị **schema/table mẫu** cho thử nghiệm CRUD.
* Chạy được **ứng dụng Node.js CRUD** trên EC2 kết nối RDS và xác nhận các thao tác **Create/Read/Update/Delete** cơ bản.
* Thực hành **CloudFormation** đúng theo lab tài liệu, theo dõi **Events** và xử lý lỗi theo hướng dẫn.
* Xác định rõ **đề tài dự án** và **bộ dịch vụ AWS** ban đầu, cân bằng giữa tính thực tế và tối ưu chi phí.
