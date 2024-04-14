---
title : "Giới thiệu"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

#### Amazon CloudFront
Amazon CloudFront là dịch vụ Mạng phân phối nội dung (Content Delivery Network) toàn cầu giúp tăng tốc phân phối nội dung trang web tĩnh và động của bạn. 
Amazon CloudFront mang đến nội dung cho bạn thông qua mạng lưới các edge location trên toàn thế giới.
Tích hợp Amazon CloudFront với các sản phẩm AWS khác để cung cấp cho các nhà phát triển và 
tổ chức một cách dễ dàng để phân phối nội dung cho người dùng cuối với độ trễ thấp, tốc độ truyền dữ liệu cao và không có những cam kết về mức sử dụng tối thiểu.

### Tổng quan về Content Delivery Network (CDN)
CDN là một hệ thống các caching server được phân phối toàn cầu nhằm tăng tốc việc tải các trang web, hình ảnh, video và các nội dung khác.
CDN sử dụng đinh vị địa lý của DNS để xác định vị trí địa lý của mỗi yêu cầu tải trang web. Sau đó, CDN truyền những nội dung đó từ caching server mà gần về vị trí hoặc nhỏ nhất về độ trễ. CDN cho phép tăng khả năng mở rộng và giảm độ trễ khi tải trang web dễ dàng để đáp ứng truy cập lưu lượng tăng đột biến.

**Amazon CloudFront chính là AWS CDN**.
Nó được sử dụng để mang nội dung của các trang web đến cho người dùng cuối nhờ vào các edge location ở khắp toàn cầu.
Khi một người dùng yêu cầu nội dung trang web nằm trong Amazon CloudFront, người dùng sẽ được định tuyến đến edge location gần nhất mà có độ trễ thấp nhất, để cho nội dung được "giao" đến nhanh nhất có thể. Nếu nội dung được yêu cầu đã có sẵn trong edge location mà có độ trễ thấp nhất, CloudFront sẽ đưa cho người dùng ngay lập tức. Nếu nội dung không có ở edge location CloudFront sẽ nhận được từ origin server. Origin server là nơi chứa các phiên bản gốc nội dung của bạn.

CloudFront được tối ưu để hoạt động tốt với các dịch vụ AWS Cloud khác như: Amazon S3 bucket, Amazon S3 static website, Amazon EC2, Elastic Load Balancing. Ngoài ra, CloudFront còn tích hợp cả Amazon Route 53. Amazon CloudFront hỗ trợ tất cả nội dung có thể được truyền qua HTTP hoặc HTTPS và còn hỗ trợ *media streaming*, sử dụng cả HTTP và Real-Time Messaging Protocol (RTMP).

