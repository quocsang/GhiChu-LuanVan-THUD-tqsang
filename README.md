# Temp-LuanVan-THUD-tqsang
Luu tru ghi chu va cac cong nghe


* Overview
- Hiện nay, cùng với sự phát triển của công nghệ, các yêu cầu về sản phẩm công nghệ cũng ngày càng tăng cao. Cùng với đó là các ứng dụng ngày càng được phát triển lớn mạnh, số lượng các tính năng, module tăng lên...Do đó, các phần mềm cung cấp hàng trăm tính năng và tất cả các tính năng điều được đóng gói trong một ứng dụng Monolithic Architecture(ứng dụng sử dụng kiến trúc một khối truyền thống) duy nhất, làm cho việc triển khai, sửa lỗi, mở rộng và năng cấp những phần mềm này trở nên khó khăn.
- Để giải quyết vấn đề đó, kiến trúc hướng dịch vụ (Service Oriented Architecture - SOA) ra đời. Nhưng SOA cũng chỉ giải quyết được một phần của vấn đề bằng các giới thiệt khái niệm "service" (một nhóm tổng hợp các tính năng tương tự trong một ứng dụng), và một phần mềm là tổ hợp của các service. Vì những quy định của SOA về giới hạn hay phạm vi của một service là khá là rộng và được định nghĩa khá "thô"(coarse-grained). Việc này đã khiến các service cũng có thể trở nên quá to và phức tạp.
- Theo đó kiến trúc dịch vụ nhỏ (Microservices Architecture) ra đời để giải quyết các vấn đề trên. Nền tảng cả kiến trúc microservices là xây dựng một ứng dụng mà ứng dụng này là tổng hợp của nhiều services nhỏ và độc lập có thể chạy riêng biệt, phát triển và triển khai độc lập.

* Deployment
Tổng quan về các công nghệ sử dụng để tạo ứng dụng theo kiến trúc Microservice
- Việc triển khai các service có một vai trò trọng yếu và gồm các yêu cầu sau:
 + Khả năng triển khai/ gỡ xuống độc lập mà không ảnh hưởng đến dịch vụ khác
 + Có thể mở rộng theo cấp microservices, chỉ mở rộng microservices cần thiết
 + Phát triển và triển khai microservices nhanh chóng
 + Một microservice ngắt kết nối hay sập thì không ảnh hưởng các dịch vụ khác
Các công nghệ có thể sử dụng giải quyết các yêu cầu trên:
+ OSGI (một nền tảng dùng để phát triển các ứng dụng theo hướng module hóa bằng java) dùng để viết các module cho từng service và quản lý các module đó.
+ Karaf (môi trường dùng để phát triển, triển khai các ứng dụng OSGI) để khởi chạy và quản lý các module, feature.
+ Docker (một công cụ mã nguồn mở cho phép lập trình viên và quản trị viên hệ thống triển khai các ứng dụng thành các containers trên môi trường Linux) cung cấp một công cụ tuyệt vời để triển khai microservices đáp ứng đủ các yêu cầu trên. 
+ ... (công cụ dùng để quản lý log)

* Scope
- Phạm vi chính là dùng để nghiên cứu các công nghệ: OSGI, Karaf, Docker dùng để xậy dựng một kiến trúc Microservice.
- Song với đó xây dựng một ứng dụng minh họa (web application) trên nền kiến trúc đã xây dựng được.
- Tổng quan về các công nghệ để xây dựng ứng dụng minh họa:
  + Back-End: Kết hợp với Spring framework dùng để sử lý.
  + Font-End: dùng Angular JS, Angula Material.
  + Một số các công nghệ liên quan: hibernate, boostraps, ...

* Result
 - Tìm hiểu và sử dụng được các công nghệ mới và nổi bật hiện nay như: OSGI, Karaf, Spring framework, Hibernate,... 
 - Tạo ra được một ứng dụng dựa trên kiến trúc Microservice bằng cách áp dụng các công nghệ đã được tìm hiểu.
