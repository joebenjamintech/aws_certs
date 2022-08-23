# ECS and Fargate cheatsheet

- ECS is a fully-managed conainer orchestration service, highly secure, reliable, and scalable way to run containers
- components of ECS
  - **cluster** multiple EC2 instances which will house the docker containers
  - **task definition** a json file that defines the config of up to 10 containers you want to run
  - **task** launches containers defined in task definition. tasks do not remain running once workload is complete
  - **services** ensures task remain running e.g. web-app
  - **container agent** binary on each EC2 instance which monitors, start and stop tasks

# ECR - elastic container registry

- ECR is a fully managed Docker container registry that makes it easy for developers to store, manage, and destroy docker container images

# Fargate

- Fargate is serverless containers, don't worry about servers. run containers and pay based on duration and consumption
  - has cold starts, so if this is an issue, use ECS
- duration is as long as you want
- memory up to 30G
- pricing, pay at least 1 minute and every additional second
