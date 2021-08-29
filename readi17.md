# AWS: S3 and Lambda

![AWS: S3 and Lambda](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2017/06/21/Step_Functions_S3_Bucket_Arch-1.png)

1. Describe “The Cloud”?

The cloud refers to software and services that run on the Internet, instead of locally on your computer. ... It's what allows you to make edits to a file in Google Docs on your home computer, and then pick up where you left off when you get to the office. Colleagues can even collaborate on the same document.

2. What is a container (as it relates to computers and servers)?

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. ... Available for both Linux and Windows-based applications, containerized software will always run the same, regardless of the infrastructure.

3. What is auto-scaling?

Autoscaling is a cloud computing feature that enables organizations to scale cloud services such as server capacities or virtual machines up or down automatically, based on defined situations such as traffic ir utilization levels.

4. What is bandwidth?

Bandwidth is the data transfer capacity of a computer network in bits per second (Bps). The term may also be used colloquially to indicate a person's capacity for tasks or deep thoughts at a point in time.

5. How do cloud providers compute service costs?

cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.



* **AWS S3** Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. Amazon S3 is designed for 99.999999999% (11 9's) of durability, and stores data for millions of applications for companies all around the world.

* **AWS Lambda Basics** AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services.

The concept of “serverless” computing refers to not needing to maintain your own servers to run these functions. AWS Lambda is a fully managed service that takes care of all the infrastructure for you. And so “serverless” doesn’t mean that there are no servers involved: it just means that the servers, the operating systems, the network layer and the rest of the infrastructure have already been taken care of, so that you can focus on writing application code.

* **AWS Lambda Functions** AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers, creating workload-aware cluster scaling logic, maintaining event integrations, or managing runtimes. With Lambda, you can run code for virtually any type of application or backend service - all with zero administration. Just upload your code as a ZIP file or container image, and Lambda automatically and precisely allocates compute execution power and runs your code based on the incoming request or event, for any scale of traffic. You can set up your code to automatically trigger from over 200 AWS services and SaaS applications or call it directly from any web or mobile app. You can write Lambda functions in your favorite language (Node.js, Python, Go, Java, and more) and use both serverless and container tools, such as AWS SAM or Docker CLI, to build, test, and deploy your functions

* **Content Delivery Network (CDN)** A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

CDNs work through servers nearest to the website visitor respond to the request. The content delivery network copies the pages of a website to a network of servers that are spread out at geographically different locations, caching the contents of the page. When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content. CDNs will also communicate with the originating server to deliver any content that has not been previously cached. In turn, the speed is improved by distributing content closer to the website visitors by using a nearby CDN server, causing visitors to experience faster page loading times. In simpler terms, for example, instead of a user in London trying to access a server in LA, which can cause slower Internet speeds, the user would be redirected through a CDN that is geographically closest to them (London, Paris, Stockholm, etc). As of today, the majority of web traffic goes through through CDNs, including traffic from major sites like Facebook, Netflix, and Amazon.
