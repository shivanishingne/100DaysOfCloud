# [Day 12/100] : Learn about the Table Viewer construct


## Cloud Research

- Installing the library:

```
npm install cdk-dynamo-table-viewer
```

- Exposing the Hit Counter table
    - edited hitcounter.ts and modified it as such `table` is exposed as a public property.
    - The we access it from the stack.

- after deploying, hit the endpoint multiple times to see the counter getting refreshed in 3 sec.

### Clean Up the Stack
- You can either delete the stack through the AWS CloudFormation console or use cdk destroy:
  ```
   cdk destroy
  ```

### Testing Constructs
- Install testing packages (I am using use the `Fine-Grained Assertions` and `Validation` type tests)
  
  ```
  npm install --save-dev jest @types/jest @aws-cdk/assert
 ```



</br>

---

</br>

## Social Proof

[twitter](link)

