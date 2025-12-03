---
title: "Worklog Tuần 3"
date: 2025-09-21
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

- Xây dựng thành công kiến trúc mạng Hybrid DNS nhằm tích hợp hệ thống DNS On-Premise (mô phỏng bằng AWS Managed Microsoft Active Directory) với dịch vụ DNS của Amazon Route 53.
- Cấu hình thành công Inbound Endpoint (cho phép truy vấn từ On-Premise đến AWS), Outbound Endpoint (cho phép truy vấn từ Route 53 Resolver ra ngoài), và Resolver Rules để định tuyến các truy vấn DNS cho các tên miền cụ thể.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Chuẩn bị và Khởi tạo hạ tầng mạng: Xem giới thiệu về Route 53 Resolver. Tạo Key Pair (ví dụ: hr-dns-key, kiểu RSA) để truy cập Remote Desktop vào EC2 Windows. Khởi tạo CloudFormation Template (ví dụ: hr-dns-vpc-stack) để xây dựng hạ tầng mạng cơ sở (VPC, Subnets, Gateway) có tính sẵn sàng cao và bảo mật. <br>  | 09/15/2025   | 09/15/2025      |
| 3   | - Hoàn tất hạ tầng và Kết nối RDGW Host: Theo dõi và đợi CloudFormation hoàn thành (khoảng 15-20 phút). Cấu hình lại Security Group trong VPC: xóa cổng không sử dụng (3391, 443) và giữ lại giao thức ICMP (IPv4) và Remote Desktop Protocol (cổng 3389). Kết nối đến Remote Desktop Gateway (RDGW) Host bằng cách tải file RDP, upload Key Pair để giải mã và lấy mật khẩu Administrator.<br>                                            | 09/16/2025   | 09/16/2025      | 
| 4   | - Thiết lập Route 53 Outbound Endpoint: Tạo Outbound Endpoint Route 53 Resolver (mũi tên đỏ) cho phép Route 53 chuyển tiếp truy vấn DNS tới hệ thống ngoài (AD). Chọn đúng VPC và Security Group. Cấu hình địa chỉ IP tự động trong hai Availability Zone (AZ). Chờ Endpoint chuyển sang trạng thái thành công <br> | 09/17/2025   | 09/17/2025      | 
| 5   | - Thiết lập Resolver Rules và Inbound Endpoint: Tạo Resolver Rule (loại Forward) để chuyển tiếp truy vấn DNS cho tên miền cụ thể (ví dụ: onprem.example.com) tới địa chỉ IP của AWS Managed Microsoft AD DNS. Tạo Inbound Endpoint Route 53 Resolver (mũi tên xanh) cho phép hệ thống DNS On-Premise (AD) truy vấn Route 53 resolver, cấu hình trong subnets riêng tư. <br>                    | 09/18/2025   | 09/18/2025      | 
| 6   | - Kiểm tra và Dọn dẹp Tài nguyên: Thử nghiệm kết quả bằng cách sử dụng lệnh nslookup onprem.example.com trên RDGW host để xác minh phân giải DNS. Kiểm tra truy vấn được định tuyến qua IP DNS Resolver của VPC (ví dụ: 10.0.0.2) và thực hiện ping tới domain môi trường truyền thống. Dọn dẹp tài nguyên: Xóa Inbound/Outbound Endpoint. Hủy liên kết (Disassociate) VPC khỏi Resolver Rule trước khi xóa Rule. Xóa AWS Managed Microsoft Active Directory, sau đó xóa CloudFormation Stacks. <br> | 09/19/2025   | 09/19/2025      | 

### Kết quả đạt được tuần 3:

- Thiết lập thành công kiến trúc DNS lai (Hybrid DNS) sử dụng Route 53 Resolver.
- Đã cấu hình Outbound Endpoint để Route 53 Resolver có thể chuyển tiếp truy vấn DNS tới hệ thống ngoài (AWS Managed AD).
- Đã tạo Inbound Endpoint cho phép hệ thống DNS On-Premise (AD) truy vấn Route 53 Resolver.
- Các Resolver Rule (loại Forward) đã được tạo để định tuyến truy vấn cho tên miền onprem.example.com tới địa chỉ IP của AWS Managed Microsoft AD DNS.
- Thử nghiệm đã xác nhận khả năng phân giải DNS hai chiều bằng lệnh nslookup trên RDGW host.
- Đã xác minh rằng truy vấn được định tuyến chính xác qua địa chỉ IP DNS Resolver của VPC (ví dụ: 10.0.0.2, theo mặc định là VPC CIDR + 2).
- Đã hoàn tất dọn dẹp tài nguyên để tránh phát sinh chi phí
