
# [Day 10/100] : Progress on the CDK workshop


### Cloud Research

- The AWS CDK is shipped with an extensive library of constructs called the AWS Construct Library. The construct library is divided into modules, one for each AWS service.

### Adding Lambda fn.
- For adding Lambda function, I needed the AWS Lambda construct library.

- To install the AWS Lambda module and all it’s dependencies into our project:
  ```
   npm install @aws-cdk/aws-lambda
  ```
  
  - By doing `cdk diff` we can see, this code synthesizes an AWS::Lambda::Function resource

Note: if `cdk deploy` command gives the following output:
```
"--require-approval" is enabled and stack includes security-sensitive updates, but terminal (TTY) is not attached so we are unable to get a confirmation from the user
```
..then try the option: 
 `cdk deploy --require-approval never`

---
### Adding API Gateway

#### Note ~
    - API Gateway will expose a public HTTP endpoint that anyone on the internet can hit with an HTTP client such as curl or a web browser.
    - Lambda proxy integration is a lightweight, flexible API Gateway API integration type that allows you to integrate an API method – or an entire API – with a Lambda function.
    - We will be using Lambda proxy integration so that any request to any URL path will be proxied directly to our Lambda function, and the response from the function will be returned back to the user.

- Installing APIg library:
  ```
  npm install @aws-cdk/aws-apigateway
  ```

 #### Troubleshooting ~
  - reasons for 5xx error returned from API Gateway:
    - Make sure your handler returns a response that includes a `statusCode`, `body` and `header` fields.
    - Degbug lambda function failure logs.

</br>

---
</br>

## Social Proof

[twitter](https://twitter.com/ImperfectShishi/status/1343914960737320960)

