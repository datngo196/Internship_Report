---
title: "Worklog Tuần 9"
date: 2025-11-02
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

- Hoàn thiện các thực hành tốt nhất về IAM bằng cách so sánh Access Keys và IAM Roles.
- Hiểu các dịch vụ cơ sở dữ liệu AWS (RDS, Aurora, Redshift, ElastiCache) và các khái niệm DB cơ bản.
- Triển khai ứng dụng web kiến trúc 2 tầng (2-tier) sử dụng Amazon EC2 và Amazon RDS.
- Thực hiện các vận hành cơ sở dữ liệu bao gồm sao lưu, khôi phục và kết nối qua RDP.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Hoàn thành Lab 44 với việc giới hạn Switch Role theo IP/Thời gian. Chuyển sang Lab 48 để thực hành tạo IAM Access Key so với việc dùng IAM Role cho EC2, qua đó hiểu tại sao Role an toàn hơn. <br>  | 10/27/2025   | 10/27/2025      |
| 3   | - Học lý thuyết Module 06 về các khái niệm cơ sở dữ liệu (OLTP/OLAP), kiến trúc Amazon RDS & Aurora, và tổng quan về các DB chuyên dụng như Redshift và ElastiCache. <br>     | 10/28/2025   | 10/28/2025      |  |
| 4   | - Bắt đầu Lab 05 (Triển khai Web App với RDS) bằng việc thiết lập nền tảng mạng: tạo VPC, cấu hình Security Group cho EC2 và RDS, tạo DB Subnet Group và khởi chạy EC2 instance.<br>  | 10/29/2025   | 10/29/2025      |  |
| 5   | - Tiếp tục Lab 05: Khởi tạo RDS database instance, cấu hình ứng dụng trên EC2 để kết nối tới database và kiểm tra việc triển khai ứng dụng web thành công. <br>    | 10/30/2025   | 10/30/2025      |  |
| 6   | - Hoàn tất Lab 05 bằng cách thực hiện sao lưu (backup) và khôi phục (restore) dữ liệu, sau đó dọn dẹp tài nguyên. Bắt đầu Lab 43 với việc học cách kết nối tới Windows instance dùng RDP Client. <br>  | 10/31/2025   | 10/31/2025      |  |

### Kết quả đạt được tuần 9:

- Thành thạo bảo mật IAM:
  - Đã triển khai các chính sách truy cập có điều kiện (dựa trên IP/Ngày giờ).
  - Chứng minh được lợi ích bảo mật của việc sử dụng IAM Roles thay vì Access Keys dài hạn.
- Triển khai Cơ sở dữ liệu:
  - Nắm vững sự khác biệt giữa các dịch vụ database của AWS (Quan hệ, Key-value, Kho dữ liệu).
  - Triển khai thành công Cơ sở dữ liệu quan hệ được quản lý (RDS) trong môi trường VPC.
- Triển khai Ứng dụng:
  - Kết nối thành công ứng dụng web trên EC2 với backend RDS instance.
  - Thực hiện các tác vụ bảo trì quan trọng như tạo bản chụp (snapshot) và khôi phục dữ liệu.
