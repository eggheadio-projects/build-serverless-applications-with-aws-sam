# Execute an AWS Lambda function locally with SAM CLI

## [Video link](https://egghead.io/lessons/aws-run-a-lambda-function-locally-with-a-custom-event-using-aws-sam-cli?pl=learn-aws-serverless-application-model-aws-sam-framework-from-scratch-baf9)

- Each time a lambda is invoked it receives an event.

- When running locally, this event will be an empty object.

- This will not usually be the case as lambda functions are designed to be triggered by events: objects uploaded to S3, people hitting endpoints, a record being deleted from dynamodb, etc.

- You can test locally with events. When you create a new SAM application, an events directory gets created as well.

- Here we can find the `event.json` file.

- We can invoke the function with this event using `sam local invoke --event ./events/event.json` and see the content.

## Resources

## Personal take

Great to be able to test specific events locally, especially if there is a consistent error you're trying to debug. This looks better than other AWS products I've used and way better than clicking around the console.
