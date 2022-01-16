How to run

Create CMK
Change CMK ARN in code
Create an S3 and lake formation full access role
Create EC2 Instance
Apply the above role to EC2
Connect to instance

#Install git #Perform a quick update on your instance: 
sudo yum update -y; 
#Install git in your EC2 instance 
sudo yum install git -y;

#Install Terraform 
sudo yum install -y yum-utils; 
sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/AmazonLinux/hashicorp.repo; sudo yum -y install terraform;

git clone https://github.com/konradbaccenture/terraform-datalake-scripts.git;

terraform init; terraform plan; terraform apply;

terraform destroy