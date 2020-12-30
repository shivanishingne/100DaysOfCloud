# [Day 11/100] : Creating our own constructs


## Cloud Research

- About the new construct:
- can be attached to any Lambda function that’s used as an API Gateway backend
- will count how many requests were issued to each URL path
- will store this in a DynamoDB table

### What is done:
- Defined a DynamoDB table with path as the partition key.
- Defined a Lambda function which is bound to the lambda/hitcounter.handler code.
- Wired the Lambda’s environment variables to the functionName and tableName of our resources.

### Debugging:
  Debugging was done from Cloudwatch logs. 

- Realised that we need to add permissions for our lambda function to read/write to the DynamoDB table.
- ALSO, we need to give our hit counter lambda the permissions to invoke the downstream lambda function.


</br>

---

</br>

## Social Proof

[twitter](https://twitter.com/ImperfectShishi/status/1344257131915005952)

