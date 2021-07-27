1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server?
*Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale*

2. List the AWS Database offerings and talk about the pros and cons of each?
- *Relational: It's good in orgnize the DB in tables and make relations between tables*
- *NoSQL: It's fast in reading the data*

3. What’s the difference between a FIFO and a standard queue?
*Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue*
*FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it*

4. How can the server be assured a message was properly received?
*by hit an event after receiving a message*

### Serverless API:
*Creates a collection of Amazon API Gateway resources and methods that can be invoked through HTTPS endpoints*

### Triggers:
*an AWS Lambda resource or resource in another service that you configure to invoke your function in response to lifecycle events, external requests or on a schedule, a function can have multiple triggers*

### Dynamo vs Mongo:
*DynamoDB is a fully managed AWS service ,supports limited data types and smaller item sizes; supports more data types and has fewer size restrictions*

### Dynamoose vs Mongoose:
*Dynamoose is a DynamoDB API structured like Mongoose, lets us provide a schema and perform CRUD operations against a DynamoDB table, installed via node and configured based on role*

## SNS (Simple Notification Service)
*Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication*

## To build Modern Apps over AWS we need :
- comput : Lambda
- Database : Dynamo DB
- Masseging : it's seinding between software componant not people

## SQS is distributed queuing service.
- Messages are not pushed to receivers. Receivers have to poll SQS to receive messages
- Messages can’t be received by multiple receivers at the same time
- Any one receiver can receive a message, process and delete it
- Other receivers do not receive the same message later.
- is mainly used to decouple applications or integrate applications.
- Messages can be stored in SQS for short duration of time (max 14 days).
- Messages can be stored in SQS for short duration of time (max 14 days).