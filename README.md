Lambda function and [Claudia](https://claudiajs.com) commands to auto-confirm new AWS Cognito users.

## Usage

1. Deploy Lambda Function

`claudia create --region [enter region] --profile [enter AWS profile] --handler index.handler`

2. Assign to Cognito UserPool

`claudia add-cognito-user-pool-trigger --profile [enter AWS profile] --user-pool-id [enter User Pool Id] --events PreSignUp`