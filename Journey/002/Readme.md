

# [Day 2/100] : Getting Started with Serverless


## Cloud Research

- Today I read about "Serverless" and Lambda functions. Topics covered include:

  1. Serverless computing
  2. Microservices
  3. Stateless functions
  4. Cold Starts
     
- AWS Lambda (Overview)
    - note: Each function runs inside a container with a **64-bit Amazon Linux AMI.**

    - the execution environment has:
      - **Memory:** 128MB - 3008MB, in 64 MB increments

      - **Ephemeral disk space:** 512MB.  This is available in the form of the /tmp directory (temporary storage).
  
      - **Max execution duration:** 900 seconds (or 15 min). So its not meant for long running processes.

      - **Compressed package size:** 50MB (packages include dependencies and stuff needed for the code to run)

      - **Uncompressed package size:** 250MB



![Lambda Function](https://github.com/shivanishingne/100DaysOfCloud/blob/main/images/anatomy-of-a-lambda-function.png)




</br>
---
</br>

## Social Proof


[Twitter]([link](https://twitter.com/ImperfectShishi/status/1340124030754406401))

