# AWS Elastic Search x Terraform

Provision [AWS Elastic Search](https://aws.amazon.com/id/elasticsearch-service/) using Terraform

## Requirements
* [Access Key](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html#Using_CreateAccessKey) to AWS
* Terraform
* Proper access to AWS stated in `~/.aws/*`

## Deploy Elastic Search using Terraform
```
# Init terraform
terraform init

# See what's the plan (you should see only add action)
terraform plan

# Apply changes
terraform apply

# type yes to continue
 ```

## Scale the Elastic Search

```
# Edit instance count https://github.com/furiatona/terra-aws-elasticsearch/-/blob/master/elk.tf#L25

# See what's the plan (you should see only change action)
terraform plan

# Apply changes
terraform apply

# type yes to continue
 ```

## Clean Up

```
# Destroy resource
terraform destroy

# type yes to continue
 ```