# AWS: S3 and Lambda
>
## What is AWS Lambda?

    AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

## How does AWS Lambda work?

    Each Lambda function runs in its own container. When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS. Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity. Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running. The customers then get charged based on the allocated memory and the amount of run time the function took to complete.

## Benefits of use Lambda

1. No servers to manage

2. Continuous scaling

3. Cost optimized with millisecond metering

4. Consistent performance at any scale

## What is CDN ?

    Content Delivery Network (CDN):A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

## Benefits of CDN

1. It speeda up the delivery of Internet content

2. It helps protect your website against certain forms of cyber attacks, such as Denial of Service attacks.

## Vocabulary terms

* **Server Instances :** instance: A virtual machine running in the cloud. server : The collection of properties and attributes that define a virtual machine that has run, will run, or is running in the cloud.

* **Containers:** A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

* **Cloud Services:** Cloud services are services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party and provide users with access to computing services such as analytics or networking via the internet.

* **Cloud Architecture:** Cloud architecture is the way technology components combine to build a cloud, in which resources are pooled through virtualization technology and shared across a network. The components of a cloud architecture include:

      * A front-end platform (the client or device used to access the cloud).

      * A back-end platform (servers and storage).

      * A cloud-based delivery model.

      * A network.

* **AWS:** Amazon Web Services is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis.

* **EC2/Beanstalk vs Heroku:**
Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. AWS Elastic Beanstalk is an orchestration service offered by Amazon Web Services for deploying applications which orchestrates various AWS services, including EC2, S3, Simple Notification Service, CloudWatch, autoscaling, and Elastic Load Balancers.
Heroku is a Platform as a Service (PaaS) product

## Preparation Materials

[AWS S3](https://aws.amazon.com/s3/)

[AWS Lambda Basics](https://www.serverless.com/aws-lambda)

[AWS Lambda Functions](https://aws.amazon.com/lambda/)

[CDN](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)
