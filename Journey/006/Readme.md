# [Day 6/100] : AWS CDK Overview


## Cloud Research

### Prerequisites
- Install CDK toolkit (using npm):
```
npm install -g aws-cdk
```

- Check toolkit version:
```
cdk --version
```

#### Creating first CDK Project
- After creating a directory, we use cdk init to create a new cdk project:
```
cdk init sample-app --language typescript
```

#### Compiling typescript code
- Since TypeScript sources need to be compiled to JavaScript, every time we make a modification to our source files, we would want them to be compiled to .js.

- Open new terminal to start watching for changes:
```
cd cdk-workshop   
```

```
npm run watch
```
- This will start the TypeScript compiler (tsc) in “watch” mode, which will monitor your project directory and will automatically compile any changes to your .ts files to .js.

#### Project Structure
> lib/cdk-workshop-stack.ts

..is where your CDK application’s main stack is defined.

> bin/cdk-workshop.ts

..is the entrypoint of the CDK application. It will load the stack defined above.

> package.json

..is your npm module manifest.

> cdk.json

..tells the toolkit how to run your app.

> tsconfig.json

.. is your project’s typescript configuration.



</br>

---
</br>

## Social Proof
- Documenting more changes in this [Github Repo](https://github.com/shivanishingne/aws-cdk-workshop) .

- [twitter](https://twitter.com/ImperfectShishi/status/1341460488647929857)

