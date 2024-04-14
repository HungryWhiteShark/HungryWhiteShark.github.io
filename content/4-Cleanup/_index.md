+++
title = "Clean up resources"
date = 2024
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

We will proceed with the following steps to delete the resources we created.

#### Delete S3 bucket

Access to [Amazon S3's interface](https://console.aws.amazon.com/s3/home)
  + Click the S3 bucket that we created before (Ex: cloudfront-bucket001)
  + Click **Empty** to delete contents inside the bucket.
  ![delete](/images/delete/001.png)

  + Write **permanently delete**, then click **Empty** to process
  ![delete](/images/delete/002.png)

  + Delete contents inside S3 bucket successfully
  ![delete](/images/delete/003.png)

  + Click **Exit**.
  + After deleting all objects in S3 bucket, click **Delete**.
  ![delete](/images/delete/003.png)

  + Enter the name of the bucket (Ex: cloudfront-bucket001) & click **Delete bucket** to delete S3 bucket itself.
  ![delete](/images/delete/004.png)


#### Delete AWS CloudFront

Access to [CloudFront's service interface](console.aws.amazon.com/cloudfront/home)
  + Click the distribution you want to delete and choose **Disable**.
  ![delete](/images/delete/005.png)

  + Click **Disable**.
  ![delete](/images/delete/006.png)

  + Wait a few minutes after disabling, click **Delete** to delete distribution.
  ![delete](/images/delete/007.png)

  + Finally, click **Delete**.
  ![delete](/images/delete/008.png)

