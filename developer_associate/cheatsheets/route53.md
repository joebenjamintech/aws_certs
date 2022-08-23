# route 53

- a DNS provider, registry and manage domains, create record sets - think godaddy or namecheap
- routing policies
  - simple routing - default routing policy, multiple addresses, result in a random endpoint selection
  - weighted routing - split up traffic based on different "weights" assigned (percentages)
  - latency based routing - direct traffic based on region, for lowest possible latency for users
  - failover routing - primary site in one location, secondary data recover site in another (change on health check)
  - geolocation routing - route traffic based on the geographic location of requests origin
  - geo-proximity routing - route traffic based on geographic location using 'bias' values (needs route53 traffic flow)
  - multi-value answer routing - return multiple values in response to DNS queries (using health checks)
- traffic flow - visual editor, for chaining routing policies, can version policy records for easy rollback
- AWS alias record - AWS smart DNS record, detects changed IPs for AWS resources and adjusts automatically
- route53 resolver - lets you regionally route DNS queries between your VPCs and you network hybrid env, can connect your on prem and cloud
- health checks can be created to monitor and automatically fail over to other endpoints, you can have healthchecks monitor other healthchecks
