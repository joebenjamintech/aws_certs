# NACL

- VPCS are automatically given a default NACL which allows all inbound and outbound traffic
- each subnet within a VPC must be associated with a NACL
- subnets can only be associated with 1 NACL at a time. associating a subment with a new NACL will remove the prev association
- if a NACL is not explicity associated with a subnet, the subnet will be automatically associated with the default NACL
- NACL has inbound and outbound rules (just like security groups)
- rule can either **allow** or **deny** traffic (unlike security groups which can only allow)
- NACLS are stateless (incoming rule will not be applied to outgoing)
- when you create NACLS, it will deny all traffic by default
- NACLS contain a numbered list of rules that gets evaluated in order from lowest to highest
- if you needed to block a single IP address you could via NACLS (security groups cannot deny)
