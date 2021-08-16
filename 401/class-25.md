# Serverless and Amplify

## Serverless Architecture

Serverless is a cloud native development model that allows developers to build and run applications without having to manage servers. A cloud provider handles the routine work of provisioning, maintaining, and scaling the server infrastructure.


Some example of available cloud services:

- AWS Lambda
- Azure Functions
- IBM OpenWhisk
- Oracle Fn Project
- Kubeless


There are many advantages of using serverless architecture over the traditional one, One of the major advantages is reduced cost. So instead of hiring a server team to maintain servers 24x7, the cost of serverless is execution-based ( only charges for the number of executions ).
but on the other hand, to be able to use serverless functions you have to access them as private APIs, and you must set up an API Gateway, and you cannot directly access them through the usual IP.

Another advantage of using serverless architecture over traditional architecture, is that setting up different environments for Serverless is as easy as setting up a single environment. You no longer need to set up dev, staging, and production machines.

Serverless architecture validity and success depends on the business requirements and not necessarily technology. In that way, serverless can be very useful when used in proper place.


## Amplify


AWS Amplify is an open-source framework fully integrated with AWS, works with GraphQL and SQL databases, and helps front-end web and mobile developers build scalable full stack applications.

There are many benefits of using it such as:

- configure backends fast
- Easily manage content
- Easy deployment
- Seamlessly connect frontends
