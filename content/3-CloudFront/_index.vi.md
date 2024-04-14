---
title : "Tạo AWS CloudFront và chặn kết nối từ một quốc gia"
date :  "`r Sys.Date()`" 
weight : 3 
chapter : false
pre : " <b> 3. </b> "
---

#### Tạo AWS CloudFront distribution

1. Truy cập vào [giao diện dịch vụ AWS CloudFront](console.aws.amazon.com/cloudfront/home)

Click vào **Create a CloudFront distribution** để tạo một CloudFront distribution.

![cloudfront](/images/cloudfront/001.png)

2. Chọn domain gốc cho AWS CloudFront. Chúng ta sẽ chọn domain gốc là S3 bucket đã được trước đó.

![cloudfront](/images/cloudfront/002.png)

3. Tại mục **Web Application Firewall (WAF)**, chọn **Enable security protections**
  ![cloudfront](/images/cloudfront/003.png)

4. Giữ các cài đặt mặc định khác và click **Create distribution**
  ![cloudfront](/images/cloudfront/004.png)

5. Hoàn thành tạo một distribution mới
   ![cloudfront](/images/cloudfront/005.png)


#### Chặn kết nối đến trang web từ một quốc gia

1. Chờ trạng thái của distribution là **Enabled**, sử dụng trình duyệt và truy cập trang web có URL là **Domain name** thêm đuôi là */index.html*.
   ![cloudfront](/images/cloudfront/006.png)

2. Có thể thấy chúng ta truy cập trang web không vấn đề gì.
   ![cloudfront](/images/cloudfront/007.png)

3. Lựa chọn distribution đang sử dụng, truy cập vào tab **Security** và click **Edit**
   ![cloudfront](/images/cloudfront/008.png)

4. Ở mục **Restriction type**, chọn **Block list**. Ở phần **Countries**, lựa chọn quốc gia mà chúng ta muốn chặn truy cập (ví dụ: Việt Nam). Sau đó click **Save changes**
   ![cloudfront](/images/cloudfront/009.png)

5. Sau khi truy cập lại trang web như trên, chúng ta sẽ không thể truy cập được. Có thể thêm nhiều quốc gia khác vào danh sách chặn
   ![cloudfront](/images/cloudfront/010.png)





