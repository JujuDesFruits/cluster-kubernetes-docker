# cluster-database-docker
Creating a cluster of noSQL (Redis/mongo) or sql (mysql/oracle)
Securing them  
Providing monitoring, backup and upgrade  

We finnaly decided to realised a project using [Vitess](https://vitess.io/overview/) because it is a cluster system for mysql who was one of our possible solution. This solution was used for big compagny as youtube, so we found that it should be revelant to work on it.
Vitess work using a kubernetes cluster so in this project there will be 4 mains tools:
* Google Cloud
* Kubernetes
* MySQL
* Vitess

## Kubernetes Cluster

here we are gonna follow the [hard way](https://github.com/kelseyhightower/kubernetes-the-hard-way) to install it, just to understand well each step used to manipulate Kubernetes

because we had custom a little bit our cluster, you can see all we did in this [folder](https://github.com/JujuDesFruits/cluster-database-docker/blob/master/KUBE-CLUSTER.md).

## MySQL

```
sudo docker run -d --restart=unless-stopped -p 80:80 -p 443:443 rancher/rancher
```
