EC2 auto scaling launches and terminates instances dynamically.
scaling is horizontal launches more instances means scale out.
provides elasticity and scalability.
Auto Scaling group is the collection of auto scaling groups that are managed together.

#### Application Load balancer
It operates at the layer 7 and it can route connection based on the layer 7 information.
Supports protocols such as HTTP and HTTPS

#### Network Load balancer
It operates at the network layer route connections based on layer 3 data it can have static ip or dynamic ip address supports protocol such as TCP and UDP

#### Gateway Load balancer
Used in front of virtual appliances such as firewall, IDS/IPS, and deep packet inspection systems.
Operates at layer 3 and listens for all traffic on all ports.
forwards traffic to the target gateway specified in the listener rules.
exchange traffic with appliances using geneve protocol on port 6081.

#### Target group
Target group are used to route request to instances that are in the target group.