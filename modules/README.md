Terraform Modules Structure
modules
|--- main.tf
|--- variables.tf
|--- output.tf

Ideal modules structure

project_terraform
|
--modules
   |
   |--vpc
   |--storages
   |--vms


To execute

Format the code in all of your files in preparation for deployment:
terraform fmt -recursive

Initialize the Terraform configuration to fetch any required providers and get the code being referenced in the module block:
terraform init

Validate the code to look for any errors in syntax, parameters, or attributes within Terraform resources that may prevent it from deploying correctly:
terraform validate
