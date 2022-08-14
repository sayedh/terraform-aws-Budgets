# Creating AWS Budgets using Terraform
In this project I used Terraform to setup a budget limit in AWS Budgets. 
![BudgetCreated](https://user-images.githubusercontent.com/30685241/184519599-8b8309c0-1b3b-4f98-8e8b-77da9d118c1f.png)

## Technologies Used
* Terraform
* AWS

## Dependencies
* Install Terraform - https://www.python.org/downloads/release/python-3106/
* Install aws cli - https://aws.amazon.com/cli/

## Executing program
* Download the repository to your computer go to project file
```
git clone https://github.com/sayedh/terraform-aws-Budgets
cd terraform-aws-Budgets
```
* Configure your aws cli using your user's access/secret keys
```
> aws configure
AWS Access Key ID [None]: ****************H64O
AWS Secret Access Key [None]: ****************cYaR
Default region name [None]: us-west-1
Default output format [None]:
```

* Now use Terraform to provision and setup the budget
```
terraform init
terraform fmt
terraform validate
terraform plan
terraform apply
```
* Now the budget is created. Go to your AWS Budgets and see the newly created budget. 


## Updating the Budget
* Change the budget details in the main.tf file
![UpdateBudget](https://user-images.githubusercontent.com/30685241/184519824-c96093c3-526d-4c74-9c66-d7ae4fdf3f8c.png)


* Now once again apply the changes
```
terraform apply
```
