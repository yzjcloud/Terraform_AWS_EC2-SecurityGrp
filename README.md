# Terraform_AWS_EC2-SecurityGrp
Build AWS EC2 Instances, Security Groups using Terraform
Terraform Modules will be used:
- Terraform module which creates VPC resources on AWS
- Terraform module which creates EC2-VPC security groups on AWS
- Terraform module which creates EC2 instance(s) on AWS

Steps:
- version.tf
- general variables
- local values (common tags)
- datasource (define ami/device type)
- VPC (variables/modules/output)
- security group (variables, bastion host SG, private SG, output)
- EC2 (variables, bastion, private, output)
   /*** private host may need put dependencies of VPC, if need to connect to the Internet***/
- elastic IP resource (dependencies on ec2/vpc)
- null resource (optional)
- .tfvars 

