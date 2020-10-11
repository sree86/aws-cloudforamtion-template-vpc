# aws-cloudforamtion-template-vpc
The cf template to launch VPC in AWS
# Usage:
You can run the aws cli command to launch cloudformation StackName
  aws cloudformation --region <region> create-stack --stack-name <stack name> --template-body file://vpc-fargate.yaml

Or You can upload the yaml file directly to the cludforamtion dashboard

# This template will create a VPC with:
1. 2 Public Subnets
2. 2 Private Subnets
3. An Internet Gateway with routes to it for Public Subnets
4. A NAT Gateway for outbound access with routes from Private Subnets set to use it
