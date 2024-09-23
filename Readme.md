# MINIKUBE__

Minikube is a lightweight Kubernetes (K8) installation, which can create a Virtual Machine (VM) on your local machine or in a cloud instance, which deploys a simple cluster containing only one node.

![image](https://github.com/user-attachments/assets/090f81c3-2106-406e-9221-64b1c4f19c4d)

1.To install Minikube on AWS EC2, we will need to use T2 Medium instance since we need at least 2 VCPUs. Remember, that T2 Medium is a paid Instance, so once you are done working, terminate the instance so that you are not charged. You can create a new key pair or use an existing one.

![39e2c328-d639-45c0-82d1-0f656d6f1938](https://github.com/user-attachments/assets/ca77096a-7ccd-427b-beab-d3a694554a1a)

 Enable HTTP and HTTPS traffic from the internet and launch the instance.



# step 1:

Go to this website:
   
curl -sL https://github.com/ShubhamTatvamasi/docker-install/raw/master/docker-install.sh | bash

![e187e2b6-0dce-40e3-bdeb-6ab84413b1b2](https://github.com/user-attachments/assets/25369b33-87af-4be3-9860-03e354f3d848)

# step 2:

sudo usermod -aG docker $USER

# step 3:

newgrp docker


# step 4:

sudo snap install kubectl --classic

# step 5:

kubectl version --client

# step 6:

curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64

![e23388a8-f10e-4545-950a-994d5e640e26](https://github.com/user-attachments/assets/d536621f-2cdb-4b24-992c-b9fe984da9e9)

# step 7:

sudo install minikube-linux-amd64 /usr/local/bin/minikube

# step 8:

minikube version

![b2351101-e2f3-4010-92f4-c380dde9f503](https://github.com/user-attachments/assets/8a79888e-15e2-4671-bdd2-75329664f251)


minikube start --driver=docker
# If you encounter root privileges error, run:

check conditions--->

minikube start --driver=docker --force

minikube status

kubectl cluster-info

kubectl config view

kubectl get nodes

kubectl get pods

minikube dashboard


#sudo apt-get install docker.io

   
3.To install driver and give the permissions to group

#minikube start --driver=docker

#sudo usermod -aG docker $USER && newgrp docker

#minikube start --driver=docker
4.Minikube is now installing Docker, and Kubernetes is installed

Congratulations. Now using Minukube, you have installed Kubernetes.

#minikube ssh

#docker ps

#exit

5.To install kubectl, we will need to install snap which is a command line utility. snap is a tool to install the containerized application

#sudo snap install kubectl --classic

#kubectl get pods

#Kubectl create namespace=django-todo-app

#kubectl get pods --namespace=kube-system

![Uploading ee69732c-dc68-4580-9b5c-3d36b2edc4fb.jpg…]()

   
