#### Policies:
Permissions are assigned using IAM policy documents that are in the JSON format.

![[Pasted image 20230106183328.png]]

#### User
one user is equal to one human being and the users should be grouped into the groups according to the job function or as per need of the admin. It is best practice for the user to inherit permissions 
from the group but we can assign them IAM policies directly to the user to give them permissions.
When a new user is created it has no permissions by default.

#### IAM Federation
IAM federation can be used to combine your existing windows active directory account with aws and it uses SAML standard.

#### Principle of least privilege
It means that to only assign permissions and privilege to the user that it needs.

#### Roles
Role are used within the aws and it allows one part of the aws to access another part of the aws. Used to allow services in aws to use another aws service. 