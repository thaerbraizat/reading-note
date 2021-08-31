# AWS: Events

![AWS: S3 and Lambda](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2017/06/21/Step_Functions_S3_Bucket_Arch-1.png)

1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server?

* Express Gateway
Express Gateway is an API Gateway that can sit at the heart of any microservices architecture, regardless of what language or platform you’re using. Express Gateway secures your microservices and exposes them through APIs using Node.js, ExpressJS and Express middleware.

* Amazon API Gateway
Amazon’s API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. With a few clicks you can create an API that acts as a “front door” for applications to access data, business logic, or functionality from your back-end services, such as workloads running on Amazon Elastic Compute Cloud (Amazon EC2), code running on AWS Lambda, or any Web application. Amazon API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, authorization and access control, monitoring, and API version management.

2. List the AWS Database offerings and talk about the pros and cons of each?

1. Relational Database. Relational databases store data with 
2. predefined schemas and relationships between them. ...
3. Amazon Aurora. ...
4. Amazon Relational Database Service (RDS) ...
5. Amazon Redshift. ...
6. Key-value Database. ...
7. Amazon DynamoDB. ...
8. In-memory Database. ...
9. Amazon ElastiCache for Memcached.

3. What’s the difference between a FIFO and a standard queue?

Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

4. How can the server be assured a message was properly received?

by listening to a received event triggered when the message received

* **SNS Javascript SDK**

![SNS Javascript SDK](https://miro.medium.com/max/821/1*dhSyZISud3pPvUmDziSy0Q.png)
![SNS Javascript SDK](https://res.cloudinary.com/practicaldev/image/fetch/s--ciMqVBs6--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://raw.githubusercontent.com/adnanrahic/cdn/master/trigger-lambda-sns/sls-aws-lambda-sns3.png)


* **SQS Javascript SDK**

![SNS Javascript SDK](https://d2908q01vomqb2.cloudfront.net/0716d9708d321ffb6a00818614779e779925365c/2020/10/23/sdk-overview-v3.png)

![SNS Javascript SDK](https://programmaticponderings.files.wordpress.com/2019/10/new-01-sqs-dynamodb-1.png)