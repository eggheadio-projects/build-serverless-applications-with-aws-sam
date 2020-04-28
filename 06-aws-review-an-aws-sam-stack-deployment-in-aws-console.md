# Review an AWS SAM stack deployment in AWS Console

## [Video link](https://egghead.io/lessons/aws-review-an-aws-sam-stack-deployment-in-aws-console?pl=learn-aws-serverless-application-model-aws-sam-framework-from-scratch-baf9)

- Once we've deployed our function, we can check on the console that all is as we'd expect.

- Console > Lambda > Applications we can review:

  - The endpoint
  - The resources
  - Monitoring - this allows us to see the relevant CloudWatch metrics without having to navigate around the (clunky) UI

- Clicking on the lambda resource we can review:

  - The function code
  - Tags (that are created by SAM)
  - Role
  - Basic settings (including timeout)

- Global values in the template.yaml can be set for all resources deployed by SAM.

- SAM is deployed using CloudFormation, so looking over there we can review:
  - All the events
  - All of the resources

Note this is the same information as found elsewhere but is helpful to have in this form.

## Resources

## Personal take

Seeing all of the resources that were created (and necessary) for a simple hello world makes the existence of CLI tools like SAM essential. Especially as AWS Console UI is pretty bad.
