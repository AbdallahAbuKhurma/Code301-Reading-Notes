# AWS: API, Dynamo and Lambda
>
## Review, Research, and Discussion

1. What are serverless functions?

    Functions that you don’t care of any things related to server just write the code

2. If you were to create a system that emulated Lambda functions, how would you do it?

    Lambda runs your function only when needed and scales automatically

3. Describe how a CDN works?

    is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user

## Document the following Vocabulary Terms

### Serverless Functions

serverless function is a programmatic function written by a software developer for a single purpose. It’s then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

### Cloud Storage

Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access.

### CDN

is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on? SQL, AUTH and API

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo? AWS

3. What are you most excited about trying to implement or see how it works? AWS

## Preparation Materials

### AWS API Gateway Overview

Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

### Benefits

* Efficient API development

* Performance at any scale

* Cost savings at scale

* Easy monitoring

* Flexible security controls

* RESTful API options

### Amazon DynamoDB

* **Amazon DynamoDB** is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. DynamoDB can handle more than 10 trillion requests per day and can support peaks of more than 20 million requests per second.

* **DynamoDB** is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

  * reliable performance even as it scales.

  * a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries.

  * a small, simple API allowing for simple key-value access as well as more advanced query patterns.

### Dynamoose

Dynamoose is a modeling tool for Amazon’s DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

## Resources

[AWS API Gateway Overview](https://www.serverless.com/amazon-api-gateway)

[AWS API Gateway](https://aws.amazon.com/api-gateway/)

[AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

[AWS DynamoDB](https://aws.amazon.com/dynamodb/)

[Dynamoose](https://dynamoosejs.com/getting_started/Introduction/)
