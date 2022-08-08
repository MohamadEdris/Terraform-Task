# Terraform_task

In this repository, i used Terraform to create the following enviroment:
- VPC
- 2 Subnets: a public and a private subnet
- Internet Gateway
- NAT Gateway
- Route Tables - one foreach subnet
- Route Tables Associations
- an instance with WordPress installed on the public subnet
- an instance with MySQL installed on the private subnet

docker was used to run mySQL and wordPress.

## Code
Create an AWS access key:
* Create an IAM user.
* Create the access key under that IAM user.
* After creating AWS access key and secret, add them to the code in TerraformFinal.tf under provider "Configure the AWS Provider" .

## Run Terraform:

clone the code:
```bash
   clone https://github.com/mohamadassi173/terraform-task
```
Go to the project directory
```bash
  cd terraform-task
```  

Replace access key and secret key in main.tf and terraform init:
```bash
   terraform init
```

preview code results:
```bash
    terraform plan
```
run:
```bash
   terraform apply
```
<img width="490" alt="image" src="https://user-images.githubusercontent.com/57872327/183362015-2e593e56-660c-4f19-9a78-0fec72e86110.png">

Screenshot of 2 created instances:  
<img width="638" alt="image" src="https://user-images.githubusercontent.com/57872327/183363158-89671f39-cd49-4270-9a3d-278aaa7a9de7.png">
