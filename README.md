# serverless-stepfunctions2
Example of deploying Step Functions backed by Serverless Lambda functions and using Cloudformation to build the Step Function.

To deploy:
1. Clone this repo to your machine
2. Edit `serverless.yml` and set your AWS Account Id under `custom.accountId`
3. Run `serverless deploy`

To run the step function:
```
# list the state machines
aws stepfunctions list-state-machines

# invoke your state machine
aws stepfunctions start-execution --state-machine-arn=ARN_OF_STATE_MACHINE_FROM_LIST_STATE_MACHINES
```
