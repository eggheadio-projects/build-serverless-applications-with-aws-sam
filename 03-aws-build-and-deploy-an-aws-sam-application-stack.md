# Build and deploy an AWS SAM application stack

## [Video link](https://egghead.io/lessons/aws-build-and-deploy-an-aws-sam-application-stack?pl=learn-aws-serverless-application-model-aws-sam-framework-from-scratch-baf9)

- We run `sam build` to build our application.

- This creates build artifacts in the `.aws-sam` directory

- We can invoke locally or deploy

- To deploy, we use `sam deploy --guided` which will ask questions which we can save

- Once we have the samconfig.toml file, we won't be asked for our details again.

- We get the resource name and the API endpoint

## Resources

## Personal take

If you've looked at Tomasz previous course in lambdas, we've pretty much achieved it all in these three lessons. This is such a much more flexible and speedy way to set up resources and get up and running with lambda.
