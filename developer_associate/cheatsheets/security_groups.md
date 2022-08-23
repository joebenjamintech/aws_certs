# security groups

- security groups act as a firewall at the instance level
- unless allowed explicity, all inbound traffic is blocked by default
- you can specify the source to either be an ip range, single ip address, or another security group
- are **stateful** - if traffic is allowed inbound, it is also allowed outbound)
- any changes to a security group take effect immediately
- ec2 instances can belong to multiple security groups
- security groups can contain multiple ec2 instances
- you **cannot block specific ip addresses** with security groups, for this you would need a network access control list (NACL)
- you can have up to 10k security groups per region
- you can have 60 inbound and 60 outbound rules per security group
- you can have 16 security groups associated to an ENI - default is 5
