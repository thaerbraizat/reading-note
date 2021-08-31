# : AWS: API, Dynamo

![AWS: S3 and Lambda](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2017/06/21/Step_Functions_S3_Bucket_Arch-1.png)

1. What are serverless functions?

serverless functions are single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. The engineering teams within those companies ensure that the serverless functions have near-perfect uptime, redundant instances around the world, and scale to any incoming network request volume.

2. If you were to create a system that emulated Lambda functions, how would you do it?

Open the Functions page on the Lambda console.
Choose Create function.
Under Basic information, do the following:
For Function name, enter my-function.
For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.
Choose Create function.

3. Describe how a CDN works?

A content delivery network (CDN) refers to a geographically distributed group
of servers which work together to provide fast delivery of Internet content.
A CDN allows for the quick transfer of assets needed for loading Internet
content including HTML pages, javascript files, stylesheets, images, and videos.
The popularity of CDN services continues to grow, and today the majority of web
traffic is served through CDNs, including traffic from major sites like 
Facebook, Netflix, and Amazon.

### AWS API Gateway Overview

Amazon API Gateway is an AWS service for creating, publishing, maintaining, monitoring, and securing REST, HTTP, and WebSocket APIs at any scale. API developers can create APIs that access AWS or other web services, as well as data stored in the AWS Cloud. As an API Gateway API developer, you can create APIs for use in your own client applications. Or you can make your APIs available to third-party app developers

API Gateway creates RESTful APIs that:
Are HTTP-based.
Enable stateless client-server communication.
Implement standard HTTP methods such as GET, POST, PUT, PATCH, and DELETE.

API Gateway creates WebSocket APIs that:

Adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server.
Route incoming messages based on message content.

### AWS DynamoDB Guide

Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability. DynamoDB lets you offload the administrative burdens of operating and scaling a distributed database so that you don't have to worry about hardware provisioning, setup and configuration, replication, software patching, or cluster scaling. DynamoDB also offers encryption at rest, which eliminates the operational burden and complexity involved in protecting sensitive data.

With DynamoDB, you can create database tables that can store and retrieve any amount of data and serve any level of request traffic. You can scale up or scale down your tables' throughput capacity without downtime or performance degradation. You can use the AWS Management Console to monitor resource utilization and performance metrics.

* Dynamoose 

Dynamoose is a modeling tool for Amazon's DynamoDB (inspired by Mongoose).
Dynamoose is Sponsored by Dynobase
Dynobase helps you accelerate your DynamoDB workflow with code generation, faster data exploration, bookmarks and more