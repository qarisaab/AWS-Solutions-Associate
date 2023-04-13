#### Simple Routing Policy
It is the policy in which you can have only one A record associated with multiple IP addresses. If you specify multiple values in a record. Route 53 return all values to the user in the random order.

#### Weighted Routing Policy
It allows you to split the traffic according to the weight. example 20% of the traffic is forwarded to the  one region and 80% is forwarded to another region.

#### Alias Record
Alias records are unique to aws it is a way of translating your domain to a resource it can be an elastic load balancer or s3 bucket.

#### CNAME Record
It allows you to translate one domain to another.