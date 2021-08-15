#Comandos de Ayuda

terraform --help 
terraform <comando> --help 

terraform version


# terraformquick


terraform init

terraform init --get-plugins=false

terraform init --verify-plugins=false


# Comandos Get

terraform get 

terraform get -update=true


#Comandos de Aprovisionamiento

terraform plan ( dry run ) 


terraform plan -destroy  Muestra un plan de destrucciòn


terraform apply Ejecuta los cambios en el entorno real 


terraform apply -target  Aplica / Despliega los cambios solo en el recurso objetivo

terraform destroy -target Destruye solo el recurso objectivo y sus dependencias

terraform refresh Reconcia el estado del archivo de estado Terraform con los recuros del mundo realv

terraform providers 


# comandos de workspaces 

terraform workspace new

terraform workspace select

terraform workspace list 


terraform workspace show 

terraform workspace delete 

# formato y vlaidacion 

terraform fmt 

terraform validate 

# Inspección de Infraestruftura


terraform graph 

terraform output 

terraform output instance_public_ip

terraform output -json 

terraform show 


# Comando de importancia

terraform import aws_instance.foo i-abcd1234

# Manipulación del estado

terraform state list 

terraform state list aws_instance.my_ec2

terraform state mv

terraform state rm 

terraform state pull

terraform state push 

terraform state show aws_instance.my_ec2 


# Comandos Miscalenso

echo "1+5" | terraform console

terraform taint aws_instance-my_ec2

terraform untaint aws_instance.my_ec2

terraform force-unlock LOCK_ID

terraform login

terraform logout 



 
