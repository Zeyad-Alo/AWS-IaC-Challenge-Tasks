# AWS Infrastructure-as-Code Challenge Tasks

Multiple challenges revolving around the use of AWS's CloudFormation to make use of IaC through preparing YAML/JSON templates and deploying them into a CloudFormation stack. Entirely executed with the AWS CLI only.

This is part of Udacity's Cloud DevOps Nanodegree in partnership with EGFWD.

## Challenge 1 - Create an EC2 instance in a given VPC
### ToDo: 
1) Write a CloudFormation script that will create a Security Group and an EC2 Instance.
2) Security Group only allows inbound access on TCP port 80 and also allows unrestricted outbound access.
3) EC2 Instance automatically deploys Apache Web Server.
```
aws cloudformation create-stack  --stack-name challenge1Stack --template-body file://challenge1.yml --parameters file://parameters.json
```


## Challenge 2 - Create the required networking IaC scripts for a new cloud environment in AWS.
### Requirements Diagram:
![img](./challenge2/req.png)
```
./create.sh infraStack infra.yml infra-param.json
```
