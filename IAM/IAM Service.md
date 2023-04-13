IAM (Identity and Access Management) service and it is the way that we can authenticate and be authorized to access services on aws.
IAM principles must be authenticated to send request
A principle is a person or application that can make request for an action or operation on  an aws resource.

### MFA
Use MFA to secure your account by using a something you know such as a password and something you have maybe a google authenticator or yubi key.

### STS 
It provides short term or temporary credentials.

### IAM policies
IAM policies are json documents that tells the identity which actions it is allowed to perform on which resources and under what conditions.
Inline policies are 1 to 1 meaning it cant be shared with other principles.

### Metadata
Instance metadata is data about your ec2 instance.
Instance meta data is at http://ip/latest/meta-data