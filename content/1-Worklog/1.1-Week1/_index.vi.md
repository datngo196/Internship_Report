---
title: "Worklog Tuần 1"
date: 2025-09-07
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Mục tiêu tuần 1:

- Nắm vững các khái niệm cơ bản về Điện toán Đám mây theo định nghĩa của AWS.
- Hiểu rõ Hạ tầng Toàn cầu (Global Infrastructure) của AWS, bao gồm Region, Availability Zone (AZ), và Edge Locations.
- Làm quen với các công cụ quản lý cơ bản (Console, IAM) và tối ưu hóa chi phí ban đầu trên AWS.
- Hoàn tất thiết lập tài khoản ban đầu theo nguyên tắc bảo mật (MFA, IAM User) và quản lý ngân sách (AWS Budget)

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Nghiên cứu định nghĩa Cloud, mô hình thanh toán, lợi ích cốt lõi (tối ưu chi phí, khả năng thêm bớt tùy ý, mở rộng toàn cầu). Nghiên cứu Hạ tầng Toàn cầu AWS (Data Center, AZ, Region, Edge Locations) <br>                         | 09/01/2025   | 09/01/2025      |
| 3   | - Thực hành tạo tài khoản AWS (xác thực email, SĐT, phương thức thanh toán). Thiết lập MFA ảo cho Root User để bảo mật <br>                                            | 09/02/2025   | 09/02/2025      | 
| 4   | - Nghiên cứu các công cụ quản lý (Console, Root/IAM User, CLI, SDK). Thực hành tạo IAM Admin Group và IAM Admin User<br> | 09/03/2025   | 09/03/2025   | 
| 5   | - Nghiên cứu các phương thức thanh toán giảm giá (On-Demand, RI, Saving Plans, Spot Instances) và mô hình Serverless. Thực hành tạo AWS Budget theo Template (ngân sách hàng tháng) <br>                    | 09/04/2025   | 09/04/2025      | 
| 6   | - Thực hành tạo Cost Budget (Custom) và Usage Budget (giới hạn theo mức sử dụng). Nghiên cứu các gói AWS Support (Basic, Developer, Business, Enterprise). Dọn dẹp tài nguyên (Clean Up Budgets) <br>                   | 09/05/2025   | 09/05/2025      |

### Kết quả đạt được tuần 1:

- Hiểu định nghĩa Cloud là việc phân phối tài nguyên CNTT theo nhu cầu qua Internet với chính sách thanh toán theo mức sử dụng (pay-as-you-go). 
- Nắm vững các lợi ích cốt lõi như tối ưu hóa chi phí (có thể tắt máy chủ vào buổi tối) và khả năng thêm bớt tài nguyên tùy ý (Scalability).
- Hiểu cấu trúc Hạ tầng Toàn cầu: Availability Zone (AZ) được thiết kế để cô lập lỗi (fault isolation), và AWS khuyến nghị triển khai tối thiểu 2 AZ để đảm bảo tính sẵn sàng cao.
- Hoàn thành việc tạo tài khoản và thiết lập bảo mật cơ bản: Đã thiết lập MFA cho Root User.
- Đã tạo IAM Admin Group và IAM Admin User, thực hiện theo best practice hạn chế dùng Root User.
- Làm quen với các mô hình chi phí: On-Demand (cao nhất), Cam kết lâu dài (RI/Saving Plans), và Tài nguyên tạm thời (Spot Instances, giảm tới 90%).
- Đã thiết lập AWS Budget để theo dõi chi phí (Cost Budget) và giới hạn mức sử dụng tài nguyên (Usage Budget).
- Phân biệt được 4 gói AWS Support cơ bản (Basic miễn phí, Developer, Business cho môi trường Production, Enterprise)
