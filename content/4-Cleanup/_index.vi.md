+++
title = "Dọn dẹp tài nguyên  "
date = 2024
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

Chúng ta sẽ tiến hành các bước sau để xóa các tài nguyên chúng ta đã tạo.


#### Xóa S3 bucket

Truy cập [giao diện quản trị dịch vụ S3](https://console.aws.amazon.com/s3/home)
  + Click chọn S3 bucket chúng ta đã tạo cho bài thực hành. (ví dụ: cloudfront-bucket001)
  + Click **Empty** để xoá nội dung bên trong bucket.
  ![delete](/images/delete/001.png)
  + Điền **permanently delete**, sau đó click **Empty** để tiến hành xóa object trong bucket.
  ![delete](/images/delete/002.png)
  + Hoàn tất xoá nội dung trong S3 bucket.
  ![delete](/images/delete/003.png)
  + Click **Exit**.
  + Sau khi xóa hết object trong S3 bucket, click **Delete**.
  ![delete](/images/delete/003.png)
  + Nhập tên của bucket (ví dụ: cloudfront-bucket001) và click **Delete bucket** để tiến hành xoá S3 bucket.
  ![delete](/images/delete/004.png)


#### Xóa AWS CloudFront

Truy cập vào [giao diện quản trị dịch vụ CloudFront](console.aws.amazon.com/cloudfront/home)
  + Click vào distribution cần xoá và chọn **Disable**.
  ![delete](/images/delete/005.png)
  + Click **Disable**.
  ![delete](/images/delete/006.png)
  + Chờ vài phút sau khi disable, click **Delete** để tiến hành xoá distribution.
  ![delete](/images/delete/007.png)
  + Click **Delete**.
  ![delete](/images/delete/008.png)

