---
title : "Introduction"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

#### Amazon CloudFront
Amazon CloudFront is a global Content Delivery Network service that accelerates the delivery of your static and dynamic web content.
Amazon CloudFront brings content to you through a network of edge locations around the world.
Integrating Amazon CloudFront with other AWS products provides developers and organizations with an easy way to deliver content to end users with low latency, high data transfer rates, and no commitments of minimum usage level.

#### Content Delivery Network (CDN) Overview
CDN is a globally distributed system of caching servers that speeds up the loading of web pages, images, videos and other contents.
CDN uses DNS geolocation to determine the geographic location of each website's request. Then, CDN transmits that content from the caching server with the closest in term of location or minimal latency. CDN enables scalability and reduced website load latency to easily accommodate traffic spikes.

**Amazon CloudFront is AWS CDN**.
It is used to bring the content of websites to end users thanks to edge locations around the globe.
When a user requests web content located in Amazon CloudFront, the user is routed to the nearest edge location with the lowest latency, so the content is delivered as quickly as possible. If the requested content is already available in the edge location with the lowest latency, AWS CloudFront will deliver it to the user immediately. If the content is not available at the edge location CloudFront will receive it from the origin server. The origin server is where the original versions of your content reside.

CloudFront is optimized to work well with other AWS Cloud services such as: Amazon S3 bucket, Amazon S3 static website, Amazon EC2, Elastic Load Balancing. Additionally, CloudFront integrates with Amazon Route 53. Amazon CloudFront supports all contents that can be transmitted over HTTP or HTTPS and also supports *media streaming*, using both HTTP and Real-Time Messaging Protocol (RTMP).


