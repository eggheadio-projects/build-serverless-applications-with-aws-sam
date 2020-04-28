# Deploy an S3 bucket and trigger an AWS Lambda function with AWS SAM

## [Video link](https://egghead.io/lessons/aws-deploy-an-s3-bucket-and-trigger-an-aws-lambda-function-with-aws-sam?pl=learn-aws-serverless-application-model-aws-sam-framework-from-scratch-baf9)

- We're going to create an S3 bucket that will trigger our lambda function any time a file is uploaded. This could be useful in file transformation (image, audio or video formatting, etc).

- In the template.yaml file, we're going to add additional resources. The spacing here is what tells SAM what level everything is on so the spacing should match the `HelloWorldFunction` above it.

```yaml
MyFilesBucket:
  Type: AWS::S3::Bucket
```

- We can run `sam build` and `sam deploy` to create the bucket.

- We can check on the console to make sure the bucket has been created.

- Now, we want to connect our Bucket to our lambda function. This should have the same indentation as the `HelloWorld` function.

```yaml
FileUpload:
  Type: S3
  Properties:
    Bucket: !Ref MyFilesBucket
    Events: s3:ObjectCreated:*
```

- We can then update our function to log out the s3 event.

```js
console.log(event.Records[0].s3);
```

- Now, we build and deploy (`sam build` and `sam deploy`).

- You can upload a file to the bucket and then check the log stream.

- It should have triggered the lambda function.

## Resources

## Personal take

I've spend a long time building monitoring things like this before and this is so quick. I'm a bit worried about the ethics of AWS but this is a the primary platform and it is quick and easy to develop on now. Also, cheap for small applications.
