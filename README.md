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

## WordPress

WordPress is a way to create websites in an open-source, modular ecosystem. It’s known as a Content Management System (CMS), which means you get an intuitive way to create and manage your posts and pages of your website.

<img width="638" alt="image" src="https://user-images.githubusercontent.com/73100170/183474584-c4bd8bbf-54a9-444c-aa2f-8583813907b2.png">


docker was used to run mySQL and wordPress.

## Code
Create an AWS access key:
* Create an IAM user.
* Create the access key under that IAM user.
* After creating AWS access key and secret, add them to the code in TerraformFinal.tf under provider "Configure the AWS Provider" .

## Run Terraform:

clone the code:
```bash
   clone https://github.com/MohamadEdris/Terraform-Task
```
Go to the project directory
```bash
  cd Terraform-Task
```  

Replace access key and secret key in TerraformFinal.tf and terraform init:
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
<img width="490" alt="image" src="https://user-images.githubusercontent.com/73100170/183473925-b25b7b8b-5088-4666-80c7-4b2196af6d44.png">


Screenshot of 2 created instances:  
<img width="638" alt="image" src="https://user-images.githubusercontent.com/73100170/183474082-e09f78e5-f043-4b93-b8e0-f7f9a912a83f.png">
