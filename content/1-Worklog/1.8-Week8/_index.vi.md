---
title: "Worklog Tuần 8"
date: 2025-10-26
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

- Làm chủ các khái niệm IAM nâng cao: Truy cập đa vùng, Chuyển đổi vai trò (Switch Role) và Kiểm soát truy cập dựa trên thuộc tính (ABAC - Tags).
- Triển khai các chính sách bảo mật hạn chế (Restriction Policies) và kiểm thử giới hạn của IAM User.
- Triển khai bảo mật dữ liệu toàn diện và kiểm toán (auditing) sử dụng KMS, CloudTrail và Amazon Athena.
- Mô phỏng các kịch bản quản lý danh tính thực tế với IAM Groups và Admin Roles.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Hoàn thành Lab 28: Tạo IAM Policy/Role, thực hành Switch Roles để truy cập tài nguyên khác vùng (Tokyo/N. Virginia) dựa trên Tag. Thực hiện Lab 30 để tạo chính sách hạn chế và test giới hạn người dùng. <br>  | 10/20/2025   | 10/20/2025      |
| 3   | - Bắt đầu Lab 33 về kiểm toán và mã hóa. Tạo các Policy, Role, Group, User cần thiết, sau đó khởi tạo khóa KMS (Key Management Service) và chuẩn bị S3 bucket để upload dữ liệu bảo mật. <br>   | 10/21/2025   | 10/21/2025      |  |
| 4   | - Hoàn tất Lab 33: Cấu hình CloudTrail để ghi log sự kiện, thiết lập Amazon Athena để truy vấn log, và kiểm thử việc chia sẻ dữ liệu đã mã hóa bằng KMS trên S3 trước khi dọn dẹp.<br>| 10/22/2025   | 10/22/2025      |  |
| 5   | - Bắt đầu Lab 44 để củng cố kiến thức cấu trúc IAM. Tạo các IAM Group và User, sau đó thực hiện kiểm tra quyền (permission checks) chi tiết để hiểu cách policy tác động đến quyền truy cập. <br>  | 10/23/2025   | 10/23/2025      | |
| 6   | - Hoàn thành Lab 44 bằng việc tạo Admin IAM Role và cấu hình cơ chế Switch Role để nâng quyền quản trị. Ôn tập lại toàn bộ kiến thức bảo mật và dọn dẹp tài nguyên. <br> | 10/24/2025   | 10/24/2025      |  |

### Kết quả đạt được tuần 8:

- Quản lý danh tính nâng cao:
  - Thực hiện thành công cơ chế Switch Role để truy cập an toàn giữa các vai trò.
  - Thực thi kiểm soát truy cập dựa trên thẻ tài nguyên (Tag) xuyên suốt các vùng AWS.
  - Quản lý quyền hạn người dùng hiệu quả thông qua Group và các chính sách hạn chế.
- Bảo mật & Tuân thủ:
  - Bảo vệ dữ liệu lưu trữ bằng mã hóa AWS KMS.
  - Thiết lập vết kiểm toán (audit trail) với AWS CloudTrail và phân tích log bằng truy vấn SQL trên Amazon Athena.
