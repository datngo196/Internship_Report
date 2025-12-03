---
title: "Worklog Tuần 4"
date: 2025-09-28
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

- Nắm vững dịch vụ Compute (EC2), các tùy chọn lưu trữ và khả năng mở rộng (Auto Scaling).
- Triển khai giải pháp bảo vệ dữ liệu sử dụng AWS Backup.
- Cấu hình lưu trữ đám mây lai (Hybrid Cloud) với AWS Storage Gateway.
- Làm chủ Amazon S3 để host website tĩnh, phân phối nội dung (CloudFront) và quản lý dữ liệu.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tìm hiểu các kiến thức cốt lõi về EC2 như Instance types, AMI, Key Pair, phân biệt EBS/Instance Store và thực hành khởi tạo máy ảo kèm cấu hình User Data. <br>            | 09/22/2025   | 09/22/2025      |
| 3   | - Học về EC2 Auto Scaling và các tùy chọn giá (Pricing), sau đó thực hiện Lab 13 để triển khai hạ tầng AWS Backup, tạo Backup plan và kiểm thử khôi phục dữ liệu. <br>                                            | 09/23/2025   | 09/23/2025      |  |
| 4   | - Hoàn thành Lab 24 bằng cách tạo EC2 cho Storage Gateway, kích hoạt Gateway và tạo File Shares. Bắt đầu Lab 57 với việc tạo S3 Bucket và tải dữ liệu mẫu lên. <br>  | 09/24/2025   | 09/24/2025      |  |
| 5   | - Tiếp tục Lab 57: Bật tính năng Static Website Hosting trên S3, cấu hình quyền truy cập công khai và thiết lập Amazon CloudFront để phân phối nội dung website. <br>                    | 09/25/2025   | 09/25/2025      |  |
| 6   | Hoàn tất Lab 57 với các tính năng nâng cao như Bucket Versioning, Lifecycle rules (di chuyển đối tượng), Sao chép đa vùng (Replication) và dọn dẹp toàn bộ tài nguyên Lab. <br> volume                                                                                         | 09/26/2025   | 09/26/2025      |  |

### Kết quả đạt được tuần 4:

- Compute (EC2):
  - Hiểu rõ sự khác biệt giữa EBS và Instance Store.
  - Biết cách sử dụng User Data để cấu hình instance khi khởi động.
  - Cấu hình được EC2 Auto Scaling và nắm được các mô hình giá của AWS.
- Data Protection:
  - Đã triển khai thành công AWS Backup để tự động hóa quy trình sao lưu và khôi phục hệ thống.
- Hybrid Storage:
  - Đã tạo và cấu hình AWS Storage Gateway để kết nối file share với cloud storage.
- Storage & CDN (S3 & CloudFront):
  - Triển khai thành công website tĩnh (Static Website) trên Amazon S3.
  - Tích hợp Amazon CloudFront để tăng tốc phân phối nội dung.
  - Thực hiện được các kỹ thuật quản lý dữ liệu: Versioning, Cross-Region Replication và Lifecycle rules.
