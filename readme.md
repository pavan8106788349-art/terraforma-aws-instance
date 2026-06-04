# Terraform AWS instance

This module creates EC2 instance in AWS

## Inputs
* project - (Required) string type, user must provide project name ex. roboshop, expense, etc.
* environment - (Required) string type, user must provide environment ex. dev, uat, prod, etc.
* ami_id - (Required) string type, user must provide ami_id of instance
* instance_type - (optional) string type, default value is t3.micro.Users can override
* sg_ids - (Required) list of string, users must provide list of security group ids instance should have
* tags - (optional) map type, users can provide tags they want to have

## Outputs
* Instance_id - ID of instance created
* public_ip - Public IP of instance created
* private_ip - Private IP of instance created