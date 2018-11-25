# cluster-database-docker
Using docker swarm  
Creating a cluster of noSQL (Redis/mongo) or sql (maria/oracle)  
Comparing them  
Securing them  
Providing monitoring, backup and upgrade  

(?) should we use [Vitess](https://vitess.io/overview/) ?

First of all we need to create a custom cluster from scartch following this [guide](https://kubernetes.io/docs/setup/scratch/).

# Kubernetes
To allow us using Vitess we must use a cluter with kubernetes.
In this case, we should have **kubectl** who serve us as controler for kubernetes manager.
```
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
echo "deb https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee -a /etc/apt/sources.list.d/kubernetes.list
sudo apt-get update
sudo apt-get install -y kubectl
```
