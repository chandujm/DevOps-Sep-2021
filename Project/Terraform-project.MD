# Objective :
* Create a complete configuration which creates ```Public & Private network```

# Network Blocks to be included :
* Create 1 Primary vpc with any cidr
* Create 1 Public subnets from primary vpc
* Create 2 Private subnets from primary vpc
* Create and attach Internet gateway with public subnet
* Create and attach Nat gateway with private subnets
* Create and associate Routing table for Public subnet and route should be enabled with Internet gateway
* Create and associate Routing table for Private subnet and route should be enabled with Nat gateways
* Create security group 
    - Inbound traffic  - allow port 22 from anywhere
    - Outbound traffic - allow all port to any destination

# Instance block to be included
* Create one ec2 instance in public subnets
* Create two ec2 instance in different private subnets
* Attach SGs with machines
  - Machine created in public subnet  - ssh should be accessible via public ip from anywhere
  - Machine created in private subnet - ssh should be accessible only between private machines not from outside.
