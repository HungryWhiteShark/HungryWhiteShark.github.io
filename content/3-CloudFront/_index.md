---
title : "Create AWS CloudFront and block access from a country"
date :  "`r Sys.Date()`" 
weight : 3 
chapter : false
pre : " <b> 3. </b> "
---

#### Create AWS CloudFront distribution

1. Access to [AWS CloudFront's interface](console.aws.amazon.com/cloudfront/home)

Click **Create a CloudFront distribution** to create a CloudFront distribution

![cloudfront](/images/cloudfront/001.png)

1. Select the origin domain for AWS CloudFront. We will choose the S3 bucket that was created before as the origin domain

![cloudfront](/images/cloudfront/002.png)

3. At **Web Application Firewall (WAF)**, select **Enable security protections**
  ![cloudfront](/images/cloudfront/003.png)

4. Remain other settings and click **Create distribution**
  ![cloudfront](/images/cloudfront/004.png)

5. Create a distribution successfully
   ![cloudfront](/images/cloudfront/005.png)


#### Block access to a static website from a country

1. Wait for the distribution's status to be **Enabled**, use the browser and access the website with the URL **Domain name** adding */index.html* at the end
   ![cloudfront](/images/cloudfront/006.png)

2. Can access the website without any problems
   ![cloudfront](/images/cloudfront/007.png)

3. Select the distribution you are using, access the **Security** tab and click **Edit**
   ![cloudfront](/images/cloudfront/008.png)

4. In the **Restriction type** section, select **Block list**. In the **Countries** section, select the country we want to block access to (for example: Vietnam). Then click **Save changes**
   ![cloudfront](/images/cloudfront/009.png)

5. After accessing the above website again, we will not be able to access it. More countries can be added to the block list
   ![cloudfront](/images/cloudfront/010.png)


