---
title: "Worklog Tuần 2"
date: 2025-09-14
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

- Đi sâu vào các dịch vụ mạng quan trọng trên nền tảng AWS.
- Thiết lập và cấu hình một môi trường Mạng ảo riêng tư (VPC) an toàn trên AWS, bao gồm việc tạo các Subnet Public và Private rải đều trên nhiều Availability Zone (AZ) để đảm bảo độ sẵn sàng cao (High-Availability).
- Nắm vững cơ chế kết nối internet cho các tài nguyên trong VPC, phân biệt vai trò của Internet Gateway (IGW) và NAT Gateway.
- Hiểu và triển khai các lớp bảo mật mạng của AWS: Network Access Control List (NACL) ở cấp độ Subnet và Security Group (SG) ở cấp độ Elastic Network Interface (ENI).
- Nghiên cứu các giải pháp kết nối mạng quy mô lớn giữa nhiều VPC, cụ thể là VPC Peering và Transit Gateway.
- Làm quen với các loại Elastic Load Balancer (ELB), tập trung vào khả năng định tuyến Layer 7 (ALB) và hiệu năng Layer 4 (NLB).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Thiết lập kiến trúc VPC cơ bản (Multi-AZ): Tạo VPC với dải CIDR cụ thể. Tạo ít nhất 4 Subnet (Public/Private trên 2 AZ khác nhau) để đảm bảo kiến trúc sẵn sàng cao. Hiểu về quy tắc 5 địa chỉ IP bị AWS giữ lại trong mỗi Subnet.<br>| 09/08/2025| 09/08/2025  |
| 3   | - Cấu hình Internet Gateway (IGW): Tạo và gắn IGW vào VPC. Tạo Route Table tùy chỉnh (Custom Route Table) cho Public Subnet. Định tuyến lưu lượng Internet (0.0.0.0/0) ra ngoài qua IGW. Liên kết Route Table này với các Public Subnet <br>                                            | 09/09/2025   | 09/09/2025      | 
| 4   | - Triển khai NAT Gateway: Phân biệt NAT Gateway và NAT Instance. Cấp phát Elastic IP. Triển khai NAT Gateway vào một Public Subnet. Cấu hình Route Table cho Private Subnet, định tuyến lưu lượng Internet (0.0.0.0/0) qua NAT Gateway, chỉ cho phép kết nối một chiều đi ra. <br>  | 09/10/2025   | 09/10/2025      | 
| 5   | - Cấu hình Bảo mật và Triển khai EC2: Nghiên cứu và phân biệt Security Group (stateful, ENI level, chỉ ALLOW) và NACL (stateless, Subnet level, ALLOW/DENY). Tạo Security Group cho máy chủ công cộng và riêng tư. Triển khai EC2 trong Public và Private Subnet. Kiểm tra kết nối giữa các Subnet và ra Internet (sử dụng Bastion Host/Jump Host concept để SSH vào Private EC2). <br>  
| 09/11/2025   | 09/11/2025   | 
| 6   | - Nghiên cứu Kết nối quy mô lớn và ELB: Tìm hiểu về VPC Peering (kết nối 1:1, không hỗ trợ transitive routing) và Transit Gateway (Hub trung tâm, kết nối số lượng lớn VPC). Khám phá Elastic Load Balancing (ELB), tập trung vào ALB (Layer 7, path-based routing) và NLB (Layer 4, hiệu năng cực cao, hỗ trợ IP tĩnh). <br>   | 09/12/2025   | 09/12/2025      | 

### Kết quả đạt được tuần 2:
- Thiết lập hoàn chỉnh một VPC: Đã tạo thành công VPC và chia các Subnet thành các tầng Public/Private trên nhiều Vùng khả dụng (AZs), đảm bảo kiến trúc High Availability (tính sẵn sàng cao).
- Nắm vững cơ chế truy cập Internet Inbound/Outbound: Đã cấu hình Internet Gateway (IGW) để cho phép truy cập Internet công cộng cho các Public Subnet.
- Bảo mật truy cập Internet cho Private Subnet: Đã triển khai NAT Gateway (đặt trong Public Subnet) và cấu hình Route Table tương ứng, cho phép các Instance trong Private Subnet chỉ có thể truy cập Internet theo chiều outbound (ra ngoài).
- Áp dụng bảo mật ở tầng mạng:
  - Phân biệt và cấu hình Security Groups (có trạng thái – Stateful, áp dụng cho ENI) và NACLs (không trạng thái – Stateless, áp dụng cho Subnet).
  - Triển khai thành công EC2 Instances trong cả Public và Private Subnets, đồng thời xác minh kết nối nội bộ và bên ngoài bằng Bastion Host (jump host).
- Nghiên cứu kết nối quy mô lớn: Hiểu rõ sự khác biệt chức năng giữa VPC Peering (kết nối 1:1) và Transit Gateway (mô hình Hub-and-Spoke, có khả năng mở rộng cao).
- Làm quen với các loại Elastic Load Balancer:
  - ALB (Application Load Balancer) dùng cho định tuyến tầng 7 (Layer 7).
  - NLB (Network Load Balancer) dùng cho hiệu năng tầng 4 (Layer 4) cực cao, cùng với các tính năng cốt lõi của chúng.
