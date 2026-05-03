---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

**Thời gian thực tập (tuần 5):** 06/04/2026 – 12/04/2026

### Mục tiêu tuần 5:

* Tiếp tục thực hành **workshop** theo tài liệu hướng dẫn.
* Bắt đầu vẽ **sơ đồ kiến trúc** cho đề tài **quản lý chi tiêu cá nhân** bằng **draw.io**.
* **Thực hành lab Amazon CloudFront** (phân phối nội dung / CDN).
* Bước đầu dựng **hạ tầng mạng VPC và Subnet** cho đồ án bằng **Terraform**.
* **Ước tính chi phí dự kiến** (theo tháng hoặc kịch bản tải) cho các **dịch vụ AWS** dự kiến dùng trong ứng dụng (đối chiếu sơ đồ kiến trúc).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tiếp tục workshop theo tài liệu (bài lab / phần đang dở).<br>- Ghi chú các điểm cần đưa vào sơ đồ kiến trúc. | 06/04/2026 | 06/04/2026 | Tài liệu workshop |
| 3 | - Cài đặt / làm quen **draw.io** (hoặc bản web).<br>- Khởi tạo sơ đồ: người dùng, frontend, API, CSDL, luồng dữ liệu chính cho ứng dụng quản lý chi tiêu cá nhân.<br>- Lưu file sơ đồ theo quy ước nhóm (tên, phiên bản). | 07/04/2026 | 07/04/2026 | [draw.io](https://www.drawio.com/) |
| 4 | - **Thực hành lab CloudFront:** tạo distribution, origin (ví dụ **S3** hoặc **ALB**), behaviour, cache policy cơ bản.<br>- Ghi lại URL endpoint và bước kiểm tra. | 08/04/2026 | 08/04/2026 | [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| 5 | - **Terraform:** khởi tạo module hoặc stack cho **VPC** (CIDR, AZ, **subnet** public/private).<br>- terraform fmt, validate, plan trên môi trường dev.<br>- Đối chiếu sơ đồ draw.io với tài nguyên định nghĩa trong code. | 09/04/2026 | 09/04/2026 | [Terraform](https://developer.hashicorp.com/terraform) |
| 6 | - Hoàn thiện phần VPC/subnet tối thiểu cho đồ án; cập nhật README hoặc comment trong code.<br>- **Ước tính chi phí dự kiến:** liệt kê dịch vụ từ sơ đồ (VPC, compute, CSDL, S3, CloudFront, xác thực, giám sát…); dùng **bảng giả định** và/hoặc **Cost Explorer** (nếu đã có tài khoản/thử nghiệm) để ước tính theo **USD/tháng**, ghi rõ giả định (region, loại instance, dung lượng, request).<br>- Rà soát chi phí tài nguyên thử nghiệm đã chạy; dọn tài nguyên không cần (nếu có). | 10/04/2026 | 10/04/2026 | [Cost Explorer](https://docs.aws.amazon.com/cost-management/latest/userguide/ce-what-is.html) |

### Kết quả đạt được tuần 5:

* Đã tiếp tục workshop theo đúng tiến độ tài liệu và nắm phần còn lại cần chuyển sang kiến trúc.

* Có bản nháp / phiên bản đầu **sơ đồ kiến trúc** (draw.io) cho đề tài quản lý chi tiêu cá nhân, thống nhất với nhóm.

* Hoàn thành phần **thực hành CloudFront** theo lab (distribution, origin, kiểm tra truy cập).

* Đã bắt đầu **Terraform** cho **VPC và subnet** phục vụ đồ án.

* Có **bảng / ghi chú ước tính chi phí dự kiến** cho các dịch vụ sẽ dùng trong ứng dụng (kèm giả định và nguồn tra giá), phục vụ so sánh phương án và kiểm soát ngân sách thử nghiệm.
