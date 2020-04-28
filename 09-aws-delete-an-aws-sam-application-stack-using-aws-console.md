# Delete an AWS SAM application stack using AWS Console

## [Video link](https://egghead.io/lessons/aws-delete-an-aws-sam-application-stack-using-aws-console?pl=learn-aws-serverless-application-model-aws-sam-framework-from-scratch-baf9)

- AWS free tier is pretty big

  - DynamoDB - 25GB free per month
  - Lambda - 1 million free requests per month

- You still can delete your SAM application, even if just to tidy up your account.

- This can be done from the console.

- Lambda -> Application -> Actions -> Delete

- This warns us that we need to go to CloudFormation and `Delete` the stack there.

- There may be problems, like if there are files in your bucket you'll have to empty those first and delete them manually.

## Resources

## Personal take

This has been something I've encountered - being redirected around the console as I've tried to delete an application. It's not always straightforward but the error messages are slightly more descriptive than I remember.
