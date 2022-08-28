# ansible-aws
DevOpsSchool test #13

Write an Ansible playbook that deploys two nodes in AWS EC2: a build node and a production node. The build node creates a Java project, the resulting artifact is transferred to and run on the production node.

<i>Before you start:</i>

You need to create a 'pass' file with an arbitrary password in the root folder of the project. 
You also need to create a file 'aws_credentials.yml', in which you specify for the AWS user:
```
aws_access_key: '<YOUR_CREDENTIAL>'
aws_secret_key: '<YOUR_CREDENTIAL>'
```
encrypt it using the password in the 'pass' file:
```
ansible-vault encrypt aws_credentials.yml --vault-pass-file pass
```