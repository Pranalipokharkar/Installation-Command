 Common Tools You Can Install Using Snap: aws cli, helm, kubectl, terraform etc.
 Snap apps auto-update in the background, so you always get the latest stable version.

#AWS CLI 
sudo snap install aws-cli --classic
aws --version
aws configure
aws configure list


#Docker



#Terraform
Official Documentation:
wget -O - https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform
terraform --version

#eksctl
curl --silent --location "https://github.com/eksctl-io/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" -o eksctl.tar.gz
tar -xzf eksctl.tar.gz
sudo mv eksctl /usr/local/bin
eksctl version

#kubectl
sudo snap install kubectl --classic
kubectl version --client





