# SNS

- SNS is a fully managed pub/sub messaging service
- for application integration, it allows decoupled services and apps to communicate with eatch other
- **topic** is a logical access point and communication channel
- a topic is able to deliver multiple protocols
- you can encrypt topics via KMS
- **publishers** use the AWS API via AWS CLI or SDK to push messages to a topic. Many AWS services integrate with SNS and act as publishers.
- **subscribers** subscribe to topics. when a topic receives a message, it automatically and immediately pushes messages to subscribers.
- all messages published to SNS are stored redundantly across multiple AZs
- the following protocols
  - **HTTP and HTTPS** create webhooks into your web-application
  - **email** good for internal email notifications (only supports **plain text**)
  - **email-json** sens you json via email
  - **amazon SQS** place SNS message into SQS queue
  - **amazon lambda** triggers a lambda function
  - **SMS** sends a text message
  - **platform application endpoints** mobile push eg. apple, google, microsoft baidu notification systems
