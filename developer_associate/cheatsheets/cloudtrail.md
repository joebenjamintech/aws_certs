# cloudtrail

- cloudtrail logs call between AWS services
- governance, compliance, operational auditing, and risk auditing are keywords relating to cloudtrail
- when you need to know **who to blame** think cloudtrail
- cloudtrail by default logs event data for the past 90s days via **event history**
- to track beyond 90 days you need to create trail
- to ensure logs have not been tampered with you need to turn on **log file validation** option
- cloudtrail logs can be encrypted usign **KMS (key management service)**
- cloudtrail can be set to log across all AWS accounts in an organization and all regions in an account
- cloudtrail logs can be streamed to cloudwatch logs
- trails are outputted to an S3 bucket that you specify
- cloudtrail logs two kinds of events: **management events** and **date events**
- **management events** log management operations e.g. AttachRolePolicy
- **data events** log data operations for resources (S3, lambda) e.g. GetObject, DeleteObject, and PutObject
- data events are **disabled** by default when creating a trail
- trail logs in S3 can be analyzed using Athena
