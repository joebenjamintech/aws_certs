# lambda

- lambda's are serverless functions - you upload your code w/o you managing or provisioning any servers
- good fit for short running tasks where you don't need to customize the os environment. if you need long running tasks (>15 mins) and a custom OS environment, then consider using **fargate**
- first 1M requests per month are free
- you can adjust the duration timeout for up to 15 mins and memory up to 3008 MB
- you can trigger lambdas from the SDK or multiple AWS services - e.g. S3, api gateway, dynamoDB
- lambda by default runs in no vpcs, to interact with some services you need to have your lambda in the same vpc. e.g. RDS
- can scale to 1000 of concurrent functions in seconds. (1000 is the default, you can increase with the AWS service limit increase)
- have cold starts (if a lambda have not been recently executed, there will be a delay)
-
