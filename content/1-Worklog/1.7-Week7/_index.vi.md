---
title: "Worklog Tuần 7"
date: 2025-10-19
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

- Hiểu cấu trúc bảo mật doanh nghiệp với AWS Organizations và Identity Center.
- Triển khai quản lý tư thế bảo mật với AWS Security Hub và mã hóa với KMS.
- Xây dựng quy trình tự động hóa phản ứng sự cố sử dụng AWS Lambda tích hợp với Slack.
- Làm chủ việc tổ chức và quản lý tài nguyên thông qua chiến lược Gắn thẻ (Tagging) và Resource Groups.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Xem các video lý thuyết về AWS Organizations, Identity Center, KMS và Security Hub. Hoàn thành Lab 18 bằng cách bật Security Hub để đánh giá điểm bảo mật và dọn dẹp tài nguyên.<br> | 10/13/2025   | 10/13/2025      |
| 3   | - Bắt đầu Lab 22 để xây dựng hệ thống phản hồi tự động. Thiết lập hạ tầng mạng (VPC, Security Groups), khởi chạy EC2 instance và cấu hình Incoming Webhook để tích hợp Slack. <br> | 10/14/2025   | 10/14/2025      |  |
| 4   | - Hoàn tất Lab 22 bằng cách tạo IAM Role cho Lambda, triển khai các hàm (functions) để tự động dừng/chạy instance và kiểm tra kết quả thông báo qua Slack trước khi dọn dẹp. <br>  | 10/15/2025   | 10/15/2025      |  |
| 5   | - Thực hiện Lab 27 tập trung vào quản lý tài nguyên. Thực hành khởi chạy EC2 kèm thẻ (tags), quản lý thẻ thông qua giao diện Console lẫn dòng lệnh CLI và lọc tài nguyên hiệu quả.<br>           | 10/16/2025   | 10/16/2025      |  |
| 6   | - Hoàn thành Lab 27 bằng việc tạo Resource Groups dựa trên thẻ và dọn dẹp tài nguyên. Bắt đầu Lab 28 với việc học cách tạo và cấu hình một IAM User an toàn. <br> | 10/17/2025   | 10/17/2025      |  |

### Kết quả đạt được tuần 7:

- Quản trị bảo mật:
  - Hiểu cách quản lý môi trường đa tài khoản với AWS Organizations và Identity Center.
  - Sử dụng AWS Security Hub để giám sát tuân thủ và các tiêu chuẩn bảo mật.
- Tự động hóa & Tích hợp:
  - Xây dựng thành công quy trình tự động hóa serverless sử dụng AWS Lambda để quản lý trạng thái EC2.
  - Tích hợp dịch vụ AWS với công cụ bên thứ ba (Slack) để giám sát thời gian thực.
- Quản lý tài nguyên:
  - Áp dụng các chiến lược gắn thẻ (tagging) nâng cao để tổ chức tài nguyên đám mây.
  - Sử dụng Resource Groups và lệnh CLI để quản lý tài nguyên số lượng lớn hiệu quả.
