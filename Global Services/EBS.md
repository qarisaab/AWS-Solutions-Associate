#### Elastic Block Store
Ebs are the storage volumes that we can attach EC2 instances with these are just the hard disk in the cloud and you can run applications on it like a regular hard disk like an OS a database or create a file system.
It is used for production workloads and it is highly available because it can be replicated within a single AZ to protect against hardware failure.
It is scalable we can dynamically increase or decrease or change the volume type with no down time or performance impact to your systems.

#### GP2
Ebs are divided into two groups one is general purpose and it is the normal boot volume that we can use it gp2 and gp3.
Then there is Provisioned IOPs (io1, 2)
These are the high performance and fast SSD it is used when we need more than 16000 IOPs 

#### IOPS
IOPs is used to measure the number of read and write operations per second it is an important metric for applications that are low latency. It has the ability to action read and writes very quickly.

#### Volumes
Volumes are virtual hard disk that goes along with the ec2 instance. This is called as the root device volume it is the volume on which our OS is installed.
EBS and EC2 goes hand in hand they will all be in the same AZ as the ec2 

#### EFS
Elastic File System is amazons NFS that is the network file system that can be mounted onto many ec2 instances at once in multiple AZs. It scales automatically as you add file to it. It uses the NFSv4 protocol.

#### FSx
Fsx for windows is shared windows storage for windows based applications 
Fsx for lustre is used for computer intensive workloads it is a file system that is used for machine learning and AI. It stores the data directly on s3.