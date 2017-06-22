# Challenge
To build the environment based on the scenario provided

Template Include :
 
 whole template is  region-agnostic (i.e. compatible with any AWS US region)

 1 VPC and  network resource required to enable the expected functionality of this challenge (e.g. route tables, internet gateway, nat gateway, subnets, etc.)


 1 classic load balancer:
- should be internet-facing with “crossZone" balancing activated.
- should route http traffic to web servers.
- set a proper health check

created 2 EC2 instances in private subnets located in different availabilityzones.

bastion host: 1 instance in a public subnet, and attach it an Elastic IP.

web servers and bastion host use EC2 key pairs that can be chosen through CloudFormation parameters.

initiate an RDS instance (db.t2.micro class with PostgreSQL) in a private subnet
