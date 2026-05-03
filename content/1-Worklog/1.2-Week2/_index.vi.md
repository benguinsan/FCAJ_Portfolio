---
title: "Worklog Tuần 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

**Thời gian thực tập (tuần 2):** 16/03/2026 – 22/03/2026

### Mục tiêu tuần 2 (theo nội dung giao tại đơn vị)

* Tìm hiểu và thực hành **VPC**, thiết lập **subnet**, **route table**, **Security Group**.
* Thực hành dựng máy chủ **EC2** trên AWS.

### Kế hoạch công việc theo ngày

| Thứ | Ngày | Nội dung công việc | Tài liệu |
| --- | --- | --- | --- |
| 2 | 16/03/2026 | VPC: CIDR, AZ, subnet public/private; **Internet Gateway** | [VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) |
| 3 | 17/03/2026 | **Security Group** và **NACL**; lab quy tắc HTTP/SSH | [Security groups](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html) |
| 4 | 18/03/2026 | **EC2**: AMI, instance type, key pair, volume **EBS** | [EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) |
| 5 | 19/03/2026 | Khởi chạy EC2 trong VPC tùy chỉnh; **Elastic IP**; **SSH** / **SSM Session Manager** | [Kết nối instance Linux](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstances.html) |
| 6 | 20/03/2026 | Lab tổng hợp: VPC + subnet + SG + EC2; checklist dọn tài nguyên | [AWS Study Group — Cloud Journey](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được trong tuần

* Thiết kế được **VPC** đơn giản kèm subnet và routing phù hợp thực hành.

* Cấu hình **Security Group** / **NACL** để kiểm soát traffic vào/ra.

* Khởi tạo và truy cập **EC2**; thực hành gắn **EBS** và xử lý lỗi cơ bản.

* Ghi lại sơ đồ lab để tái sử dụng cho đồ án nhóm và các workshop sau.
