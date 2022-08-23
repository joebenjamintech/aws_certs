# auto scaling groups (ASG)

- an ASG is a collection of EC2 instances grouped for scaling and management
- scaling out is when we add servers
- scaling in is when you remove servers
- scaling up is when you increase the size of an instance (e.g. updating launch config w/ larger size)
- size of an ASG is based on min, max and desired capacity
- **target scaling policy** scaled based on when a target value for a metric is breached e.g. Average CPU Utilization exceed 75%
- **simple scaling** policy triggers a scaling when an alarm is breached
- **scaling policy w/ steps** is the new version of simple scaling policy and allows you to create steps based on eculation alarm values
- desired capacity is how many EC2 instances you want to ideally run
- an ASG will always launch instances to meet mimimum capacity
- health checks determin current state of an instance in the ASG
- health checks can be run against either an ELB or the EC2 instances
- when an autoscaling launches a new instance it use a launch config which holds the config values for the new instance e.g. AMI, instancetype, role
- launch configs cannot be edited and must be cloned or a new one created
- launch configs must be manually updated by editing the auto scaling settings
