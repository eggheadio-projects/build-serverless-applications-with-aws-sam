# Execute an AWS Lambda function locally with SAM CLI

## [Video link](https://egghead.io/lessons/aws-execute-an-aws-lambda-function-locally-with-sam-cli?pl=learn-aws-serverless-application-model-aws-sam-framework-from-scratch-baf9)

- We often want to test our code without pushing it to AWS to test.

- We need to have built our function before we do that with `sam build`

- Then we can run `sam local invoke`.

- If you have more than one function, you have to provide the name.

- You'll need to have Docker up and running locally for this to work but that was part of the SAM installation instructions

- The first time you run a function, Docker will need to fetch the relevant image so this will take a while to download before you can experience the benefits of this speed increase.

- If you have the code editor toolkit installed, you can click `Run locally` to invoke the function straight from there.

## Resources

## Personal take

Noice! So many times I've been debugging lambdas, uploading to AWS and waiting for that process only to find my next solution didn't work. This is so much faster and so useful!
