# infrastructure
Git repository for Infrastructure as code setup

#Steps for creating a cloud formation template

Create a cloud formation template for creating VPC, Internet Getway, Subnets etc

# Create the cloud Formation template using follwing command

aws cloudformation create-stack --stack-name VPCStack1 --template-body file://cloudformation.json --parameters file://parameter.json --region us-east-1 --profile awsdev

# delete cloud formation stack using following command

aws cloudformation delete-stack --stack-name VPCStack1 --region us-east-1 --profile awsdev

# Importing ssl certificate into ACM
aws acm import-certificate --certificate file://mycert.pem --certificate-chain file://prod_shubhamkawane_me.ca-bundle --private-key file://server.private.pem --profile awsprod


