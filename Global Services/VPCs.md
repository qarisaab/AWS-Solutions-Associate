#### VPCs
Virtual Private Cloud is a virtual data center in the cloud. It is logically isolated part of the cloud where the user can define it own network control and it gives you complete control of the virtual networks. It consists of internet gateways and route tables, access control lists and subnets.
1 subnet is always in one AZ. 
1 key thing is that the security groups are stateful meaning that the request from the instance will be allowed even if the inbound connections are not allowed it differs here from the access lists.

#### Network ACLs
VPC automatically come with acls that by default allows all traffic in and out. Custom acls block all traffic by default so we need to add rules and then associate it with a specific subnet.
An ACL can be associated with multiple subnets but the subnets must use only one ACL . When you associate it with more than one acls it will override the previous acl