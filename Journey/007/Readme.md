# [Day 7/100] : CDK continued


## Cloud Research

####  Synthesize a template from your app
-  When CDK apps are executed, they produce (or “synthesize”) an AWS CloudFormation template for each stack defined in your application
  ```
  cdk synth
  ```
  - `The AWS::CDK::Metadata` resource is automatically added by the toolkit to every stack. It is used by the AWS CDK team for analytics and to allow us to identify versions with security issues.

#### Bootstrap stack
- A "bootstrap stack" can be installed when deploying the cdk app for the first time.  This stack includes resources that are used in the toolkit’s operation (eg, S3 bucket that stores templates and asses during deployment process)
```
 cdk bootstrap
```

- Note: If you get "Access Denied" error, then check whether AWS CLI is set up correctly, or if the active AWS profile does not have the `cloudformation:CreateChangeSet` permission.

#### CDK Deploy
- To deploy the cdk app:
  ```
  cdk deploy
  ```
  
  - Note: we will get a warning in the console
  -  output should be in the format:
     
  `Stack ARN:
arn:aws:cloudformation:REGION:ACCOUNT-ID:stack/CdkWorkshopStack/STACK-ID`


- Each CDK stack maps 1:1 with CloudFormation stack.
  


</br>

---

</br>

## Social Proof

[twitter](https://twitter.com/ImperfectShishi/status/1341969885316796416)

