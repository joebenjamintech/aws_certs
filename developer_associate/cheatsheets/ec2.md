# EC2

- a cloud computing service
- configure you EC2 by choosing your OS, storage, memory, network throughput
- launch and SSH into your server within minutes
- EC2 comes in variety instance types specialize in different roles:
  - **general purpose** balance of compute, memory and networking resources
  - **compute optimized** ideal for compute bound applications that benefit from high performance processor
  - **memory optimized** fast performance for workloads that process large data sets in memory
  - **accelerated optimized** hardware accelerators, or co-processors
  - **storage optimized** high, sequential read and write access to very large data sets on local storage
- instance sizes **generally double** in price and key attributes
- **placement groups** let you to choose the logical placement of your instances to optimize for communication, performance or durability. placement groups are free
- **userdata** a script that will automatically run were launching an EC2 instance
- **metadata** meta data about the current instance, you can access this meta data via local endpoint when SSH'd into the EC2 instance e.g. curl http://169.254.169.254/latest/meta-data meta data could be the instance type, current ip address etc.
- **instance profiles** a container for an IAM role that you can use to pass role information to an EC2 instance when the instance starts
