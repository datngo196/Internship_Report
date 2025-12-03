---
title: "Worklog Tuần 5"
date: 2025-10-05
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

- Làm chủ các tính năng nâng cao của Amazon S3 (Storage Classes, Lifecycle, Access Points) và Glacier.
- Hiểu về giải pháp Hybrid Cloud sử dụng AWS Storage Gateway và Snow Family.
- Thực hiện di chuyển máy ảo từ on-premise lên AWS (VM Import/Export).
- Triển khai và quản lý hệ thống tệp Windows File Server (FSx) với cấu hình Multi-AZ.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Xem các video lý thuyết Module 04 về S3 Storage Classes, Access Point, Static Website, CORS và Snow Family, sau đó bắt đầu Lab 13 bằng việc tạo S3 bucket và triển khai hạ tầng backup. <br>  | 09/29/2025   | 09/29/2025      |
| 3   | - Hoàn thành Lab 13 với việc cài đặt thông báo (notification) và test khôi phục dữ liệu, sau đó chuyển sang Lab 14: chuẩn bị VMWare Workstation và xuất máy ảo từ môi trường local. <br>          | 09/30/2025   | 09/30/2025      |  |
| 4   | - TTiếp tục Lab 14: Upload máy ảo lên AWS, import thành AMI và khởi chạy instance; tiến hành làm Lab 24 để khởi tạo dịch vụ Storage Gateway. <br>  | 10/01/2025   | 10/01/2025      | |
| 5   | - Hoàn tất Lab 24 bằng cách tạo File Shares và mount ổ đĩa xuống máy local, sau đó bắt đầu Lab 25 để tạo hệ thống file SSD và HDD Multi-AZ (FSx). <br>                    | 10/02/2025   | 10/02/2025      | |
| 6   | - Hoàn thành việc thiết lập hệ thống file Multi-AZ trong Lab 25, ôn tập lại toàn bộ kiến thức lưu trữ trong tuần và dọn dẹp sạch sẽ tài nguyên (S3, Gateway, File System) để tránh phát sinh phí. <br>   | 10/03/2025   | 10/03/2025      |  |

### Kết quả đạt được tuần 5:

- Lưu trữ nâng cao:
  - Hiểu sâu về hiệu năng S3, bảo mật (CORS/ACL) và chiến lược lưu trữ lâu dài với Glacier.
  - Nắm được quy trình chuyển dữ liệu offline với AWS Snow Family.
- Backup & Di chuyển:
  - Cấu hình thành công thông báo cho AWS Backup và kiểm thử quy trình khôi phục.
  - Thực hiện thành công việc di chuyển máy ảo VMWare từ dưới hạ tầng local lên AWS EC2.
- Hybrid & File Systems:
  - Kết nối lưu trữ giữa on-premise và cloud thông qua AWS Storage Gateway.
  - Triển khai hệ thống file Windows (FSx) với độ sẵn sàng cao (Multi-AZ) trên cả SSD và HDD.
