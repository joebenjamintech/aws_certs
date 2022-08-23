# vcp endpoints

* VCP endpoints help keep traffic between AWS servics within the AWS network
* there are two kinds of VPC endpoints, interface, endpoints and gateway endpoints
* interface endpoints **cost money**, gateway endpoints **are free**
* interface endpoints uses an elastic network interface (ENI) with private IP (powered by AWS privatelink)
* gateway endpoings is a target for a specific route in your route table
* interface endpoints support many AWS services
* gateway endpoint only support dynamodb and S3
