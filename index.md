## Reference Architectures on AWS

#### Build a simple web application 

If you just have a simple web application with some static and dynamic content, you could follow the architecture [here](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/web-application.html)  


![Serverless Web App Architecture!](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/images/image7.png "Serverless Web App Architecture")

You can easily build the architecture using the CDK solution construct at [AWS-Serverless-Webapp](https://github.com/awslabs/aws-solutions-constructs/tree/main/source/use_cases/aws-serverless-web-app)

#### Build a Restful Microservice

It is easy to build a Restful service with serverless components such as the API Gateway and Lambda functions as described [here](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/restful-microservices.html)

![Restful Microservice!](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/images/image2.png "Restful Microservice")


It is possible to build this service using the API-Gateway-Lambda module with AWS Solution Constructs [https://github.com/awslabs/aws-solutions-constructs/tree/main/source/patterns/%40aws-solutions-constructs/aws-apigateway-lambda](https://github.com/awslabs/aws-solutions-constructs/tree/main/source/patterns/%40aws-solutions-constructs/aws-apigateway-lambda)

#### Build a Mobile backend

A mobile backend can be implemeneted using a similar approach such as the Rest api service above, but sometimes one needs to simplify communication with the backend and add capabilities such as realtime updates, offline capability, etc. Ths can be achived using graphql technology as indicated [here](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/mobile-backend.html)

![Mobile Backend!](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/images/image5.png "Mobile Backend")

Check out the blog [Building Scalable GraphQL APIs on AWS with CDK, TypeScript, AWS AppSync, Amazon DynamoDB, and AWS Lambda](https://aws.amazon.com/blogs/mobile/building-scalable-graphql-apis-on-aws-with-cdk-and-aws-appsync/) to understand how to build a full stack appsync backend using the cloud development kit (CDK)

#### Stream Processing 

Some of the application above would require additional capabilities such as processing click-stream data for analysis. This is also possible on AWS using a fully serverless stack as described [here](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/stream-processing.html)

![Stream Processing!](https://docs.aws.amazon.com/wellarchitected/latest/serverless-applications-lens/images/image6.png "Stream Processing")

For a solution on how you can deploy this on AWS using CDK code, review the blog [Build a real-time streaming analytics pipeline with the AWS CDK](https://aws.amazon.com/blogs/big-data/build-a-real-time-streaming-analytics-pipeline-with-the-aws-cdk/)