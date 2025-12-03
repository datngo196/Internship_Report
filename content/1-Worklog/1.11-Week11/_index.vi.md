---
title: "Worklog Tuần 11"
date: 2025-11-16
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

- Làm chủ thiết kế và vận hành cơ sở dữ liệu NoSQL với Amazon DynamoDB (Sao lưu, Global Tables).
- Triển khai chiến lược phân bổ chi phí sử dụng Tagging và các công cụ quản lý chi phí.
- Sử dụng các công cụ lập trình AWS (CloudShell, SDK) để quản lý tài nguyên bằng mã lệnh.
- Thực hiện chuẩn bị, hồ sơ hóa (profiling) và làm sạch dữ liệu trực quan với AWS Glue DataBrew.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Đi sâu vào Amazon DynamoDB (Lab 39): Khám phá giao diện console, thực hiện sao lưu/khôi phục và nghiên cứu các mẫu thiết kế nâng cao cho ứng dụng serverless toàn cầu. <br>  | 11/10/2025   | 11/10/2025      |
| 3   | - Hoàn thành Lab 40 về Phân bổ chi phí: Xây dựng cơ sở dữ liệu, nạp dữ liệu, áp dụng chiến lược gắn thẻ (tagging) để theo dõi mức sử dụng và truy vấn chi phí. <br>      | 11/11/2025   | 11/11/2025      |  |
| 4   | - Thực hiện Lab 60 để thực hành quản lý tài nguyên AWS thông qua giao diện dòng lệnh: Amazon CloudShell và AWS SDK, hiểu rõ sự khác biệt giữa thao tác trên Console và qua code.<br>  | 11/12/2025   | 11/12/2025      |  |
| 5   | - Bắt đầu Lab 70 về chuẩn bị dữ liệu: Khởi tạo môi trường Cloud9, tải và upload dataset lên S3, thiết lập AWS Glue DataBrew và chạy profiling để đánh giá chất lượng dữ liệu. <br>        | 11/13/2025   | 11/13/2025      |  |
| 6   | - Hoàn tất Lab 70 bằng việc làm sạch và chuyển đổi dữ liệu với DataBrew recipes. Tiếp tục Lab 72 để thu thập, lưu trữ và tạo danh mục dữ liệu (Catalog) trên AWS Glue, sau đó dọn dẹp tài nguyên. <br> | 11/14/2025   | 11/14/2025      |  |

### Kết quả đạt được tuần 11:

- Cơ sở dữ liệu Serverless (NoSQL):
  - Thành thạo các khái niệm cốt lõi của DynamoDB và kiến trúc hướng sự kiện.
  - Triển khai được chiến lược sao lưu cho dữ liệu NoSQL.
- Quản lý & Chi phí:
  - Áp dụng hiệu quả chiến lược gắn thẻ (tagging) để theo dõi chi phí chi tiết.
  - Chứng minh khả năng tương tác với AWS thông qua CLI/SDK trên CloudShell.
- Kỹ thuật dữ liệu (Data Engineering):
  - Sử dụng AWS Glue DataBrew để chuẩn hóa và làm sạch dữ liệu thô mà không cần viết code.
  - Xây dựng được danh mục dữ liệu nền tảng cho các quy trình phân tích.