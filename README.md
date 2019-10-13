# springboot-terraform
springboot-terraform

Stpes to deploy the appliaction in AWS cloud.
=============================================

1-infrastructure
=================
terraform init -backend-config="infrastructure-prod.config"

terraform plan -var-file="production.tfvars"

terraform apply -var-file="production.tfvars"

terraform destroy -var-file="production.tfvars"




2-platform
=============

terraform init -backend-config="platform-prod.config"

terraform plan -var-file="production.tfvars"


terraform apply -var-file="production.tfvars"

terraform destroy -var-file="production.tfvars"


3.aplication
=============
1. sh deploy.sh build
2. sh deploy.sh dockerize
3. sh deploy.sh deploy
4. sh deploy.sh destroy



Final output URL
=================


https://springbootapp.ankamma-springboot-test.com/test
