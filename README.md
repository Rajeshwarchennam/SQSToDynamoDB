# Pushing SQS messages to DynamoDB
## Objective
Considering there is continuous traffic of messages to SQS, our goal is store the messages in DynamoDB
## Architecture
* Use a python script (host it on AWS EC2 instance) to send messages continuously to SQS.
* Create a lambda function which gets triggered by the SQS Messages. 
* This lambda function starts populating those messages to DynamoDb and write logs to AWS CloudWatch
## HLD Architecture Diagram
![alt text](https://github.com/Rajeshwarchennam/SQSToDynamoDB/blob/master/SQStoDynamoDbArchitecture.png)
