# Deploy a new DynamoDB table to AWS using AWS SAM template

## [Video link](https://egghead.io/lessons/aws-deploy-a-new-dynamodb-table-to-aws-using-aws-sam-template?pl=learn-aws-serverless-application-model-aws-sam-framework-from-scratch-baf9)

- We're going to dine a new DynamoDB and deploy it with SAM.

- This is a new resource in our `template.yaml` file.

```yaml
MyAwesomeTable:
  Type: AWS::Serverless::SimpleTable
  Properties:
    PrimaryKey:
      Name: id
      Type: String
    TableName: my-awesome-database
```

- We don't need to give any properties for a simple table but we can.

- The indentation should be one below the `Resources` level.

- We can build, deploy and check in the console that is has all been setup.

- In the DynamoDB console, we can see that to add a new item to `my-awesome-database` we have to provide a primary key called `id` and it has to be a `String` - just like our yaml said.

## Resources

## Personal take

This was quick and easy - and great to debug if stuff goes wrong. Again, the console is less than ideal for these kind of operations and there are a lot options that you need to set correctly. SAM takes a lot of the friction out of that process.
