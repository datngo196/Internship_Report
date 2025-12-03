---
title: "Worklog Tuần 10"
date: 2025-11-09
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

- Thực hiện di chuyển cơ sở dữ liệu đa dạng (SQL Server/Oracle sang Aurora MySQL) sử dụng AWS SCT và DMS.
- Xử lý sự cố trong các kịch bản di chuyển phức tạp liên quan đến chuyển đổi cấu trúc, áp lực bộ nhớ và lỗi bảng.
- Xây dựng đường ống phân tích dữ liệu Serverless sử dụng Amazon Kinesis, Glue và Athena.
- Trực quan hóa dữ liệu kinh doanh (BI) sử dụng Amazon QuickSight.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Bắt đầu Lab 43: Kết nối thông qua EC2 Fleet Manager, cấu hình cơ sở dữ liệu Nguồn (SQL Server/Oracle), xử lý các ràng buộc (constraints) và chuẩn bị môi trường Đích Aurora MySQL.<br>  | 11/03/2025   | 11/03/2025      |
| 3   | - Tiếp tục Lab 43: Sử dụng công cụ Schema Conversion Tool (SCT) để chuyển đổi cấu trúc bảng, tạo các Migration Task, Endpoint và khởi chạy quy trình Serverless Migration. <br>   | 11/04/2025   | 11/04/2025      |  |
| 4   | - Hoàn tất Lab 43 bằng cách giám sát log, xử lý lỗi (troubleshoot) các kịch bản test như Tràn bộ nhớ (Memory Pressure), Lỗi bảng, kiểm tra dữ liệu và dọn dẹp tài nguyên. <br>  | 11/05/2025   | 11/05/2025      | |
| 5   | - Bắt đầu Module 07 (Lab 35): Thiết lập lớp thu thập dữ liệu bằng cách tạo S3 Bucket, cấu hình Kinesis Data Firehose Delivery Stream và tạo dữ liệu mẫu để phân tích. <br>   | 11/06/2025   | 11/06/2025      |  |
| 6   | - Hoàn thành Lab 35: Cấu hình AWS Glue Crawler để tạo danh mục dữ liệu, thực hiện truy vấn SQL với Amazon Athena, trực quan hóa dữ liệu trên QuickSight và dọn dẹp tài nguyên. <br> | 11/07/2025   | 11/07/2025      |  |

### Kết quả đạt được tuần 10:

- Di chuyển Cơ sở dữ liệu (Migration):
  - Thực hiện thành công việc di chuyển dữ liệu từ các nguồn khác nhau (SQL Server, Oracle) sang AWS Aurora MySQL.
  - Sử dụng thành thạo AWS Schema Conversion Tool (SCT) và Database Migration Service (DMS).
  - Có kinh nghiệm xử lý sự cố khi migration thất bại (lỗi bộ nhớ, lỗi ánh xạ bảng).
- Đường ống Phân tích dữ liệu (Analytics):
  - Xây dựng thành công pipeline dữ liệu serverless: Thu thập (Kinesis) -> Lưu trữ (S3) -> Danh mục hóa (Glue).
  - Phân tích tập dữ liệu lớn bằng truy vấn SQL trên Amazon Athena mà không cần quản lý máy chủ.
- Business Intelligence:
  - Kết nối Amazon QuickSight với nguồn dữ liệu để tạo các báo cáo trực quan tương tác.