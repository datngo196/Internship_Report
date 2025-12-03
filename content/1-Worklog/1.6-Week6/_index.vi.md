---
title: "Worklog Tuần 6"
date: 2025-10-12
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

- Làm chủ quản trị nâng cao Amazon FSx for Windows File Server (Hiệu năng, Chống trùng lặp, Hạn ngạch).
- Triển khai website tĩnh toàn cầu sử dụng Amazon S3 và Amazon CloudFront.
- Thực hiện các chiến lược bảo vệ dữ liệu trên S3 (Versioning, Replication, Lifecycle).
- Hiểu nền tảng về Bảo mật AWS, Định danh và Quản lý truy cập (IAM & Cognito).
### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Đi sâu vào các tính năng nâng cao của Lab 25 bao gồm tạo file shares, kiểm tra và giám sát hiệu năng, bật tính năng chống trùng lặp dữ liệu (deduplication), shadow copies, quản lý phiên người dùng và hạn ngạch lưu trữ. <br>  | 10/06/2025   | 10/06/2025      |
| 3   | - Hoàn tất Lab 25 bằng việc thực hành mở rộng băng thông (throughput) và dung lượng lưu trữ, sau đó xóa môi trường. Bắt đầu Lab 57: tạo S3 bucket, tải dữ liệu và bật tính năng Static Website Hosting.<br>         | 10/07/2025   | 10/07/2025      |  |
| 4   | - Tiếp tục Lab 57: Cấu hình chặn truy cập công khai và các đối tượng công khai, sau đó thiết lập và kiểm thử Amazon CloudFront để phân phối nội dung website với độ trễ thấp.<br> | 10/08/2025   | 10/08/2025      |  |
| 5   | - Hoàn thành Lab 57 với các tác vụ quản lý dữ liệu: bật Bucket Versioning, di chuyển đối tượng theo Lifecycle rules, cấu hình sao chép đa vùng (Multi-Region Replication) và dọn dẹp tài nguyên. <br>        | 10/09/2025   | 10/09/2025      |  |
| 6   | - *Bắt đầu Module 05: Nghiên cứu Mô hình Trách nhiệm Chia sẻ (Shared Responsibility Model), tìm hiểu các khái niệm cốt lõi của AWS IAM và tổng quan về Amazon Cognito. <br> | 10/10/2025   | 10/10/2025      |  |

### Kết quả đạt được tuần 6:

- Lưu trữ tệp nâng cao (FSx):
  - Đã cấu hình các tính năng tối ưu lưu trữ như Data Deduplication và Shadow Copies.
  - Quản lý kiểm soát truy cập thông qua user sessions và storage quotas.
  - Thực hiện thành công việc mở rộng băng thông và dung lượng lưu trữ.
- Phân phối nội dung & S3:
  - Host thành công website tĩnh trên S3 và tăng tốc truy cập bằng CloudFront CDN.
  - Triển khai các chiến lược vòng đời và bảo vệ dữ liệu (Versioning, Replication).
- Nền tảng bảo mật:
  - Nắm vững Mô hình Trách nhiệm Chia sẻ giữa AWS và khách hàng.
  - Hiểu vai trò của IAM trong kiểm soát truy cập và Cognito trong quản lý định danh người dùng.