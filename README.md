# ft_service
## This is a System Administration and Networking project.


  > Kebernetes + load balancer + dockerfile +Nginx + worldpress + phpMyadmin + FTPS + Minikube

 ## what is kubernetes ?! 
→Kubernetes, also known as K8s, is an open-source system for automating deployment, scaling, and management of containerized applications. groups containers that make up an application into logical units for easy management and discovery.
<br>
Why we use Kubernetes : 
<br>
- Manage hundreds of containers.
- Increased usage of containers.
- High Availability "always running"
- Scalability "high performance" + faster
- Backup and restore.
 <br>
→In Kubernetes, you have:
 <br>
- Pod Smallest Unit in K8s, it creates a running env A pod is a running instance of a deployment, you can run a shell into it. It has its own IP       and its own memory space, Pods connect with each other using services.
 <br>
  - Services an object that links a deployment externally or to other containers. For example, a deployment that will link the IP 192.168.0.1 to the 10 Apache servers and pick the one that has the least workload.
<br>
- Volumes it attaches physical storage in ur hard drive that storage can be in a local machine or remote storage  outside k8s
if u want to take ur local application and release it to ur Users yo use a Web Server,
<br>
- Deployment is an object in Kubernetes that helps you to manage a group of identical pods. without a deployment, you’d got to produce, update, and delete a bunch of pods manually.

<a href="https://ibb.co/QF0PGPN"><img src="https://i.ibb.co/PZkc8ch/Screen-Shot-2021-03-25-at-11-18-50-AM.png" alt="Screen-Shot-2021-03-25-at-11-18-50-AM" border="0"></a>
## what is Minikub ?! :thought_balloon:
Minikube it'as one Node Cluster, whew the Master processes and Work processes work on the same Node (One Machine), like (Mini-Cluster). <br>
- It will create avirtual BOX on ur laptop.
- Node Run in that  virtual Box <br>
-> :running_woman: To Run  or to config that mini-cluster , You gonna need Kublet or what we call as a Comand line "Kubctl".
<br>
- The Kubelet is the star :star2:	 of the show on every node. It’s the main Kubernetes agent, and it runs on every node in the cluster. In fact, it’s common to use the terms node and kubelet interchang eably,When you join a new node to a cluster, the process installs kubelet onto the node. The kubelet is then responsible for registering the node with the cluster.
<br>
 - Kube-proxy :The last piece of the node puzzle is the kube-proxy. This runs on every node in the cluster and is responsible for local cluster networking. For example, it  makes sure each node gets its own unique IP address, and implements local IPTABLES or IPVS rules to handle routing and load-balancing of traffic on the Pod network.
 <br>
  :nerd_face: For Better Understanding + instaling minikube + use kubctl : https://www.youtube.com/watch?v=X48VuDVv0do
 
 ## what's Load Blancer  :libra: 
 - Load balancing is the process of efficiently distributing network traffic among multiple backend services, and is a critical strategy for maximizing scalability and availability.

 ## what's MetalB :question:
 - MetalLB is a great load balancer for a home Kubernetes cluster. It allows you to assign real IPs from your home network to services running in your cluster and access them from other hosts on your home network.
## What is Grafana & What Is It Used For?
Grafana is an open source solution for running data analytics, pulling up metrics that make sense of the massive amount of data & to monitor our apps with the help of cool customizable dashboards.
Grafana connects with every possible data source, commonly referred to as databases such as Graphite (Graphite, again, is a monitoring tool), Prometheus, Influx DB (InfluxDB is a time series database designed to handle high write and query loads.), ElasticSearch, MySQL, PostgreSQL etc.

<a href="https://ibb.co/nzFZPjb"><img src="https://i.ibb.co/qkvXJpd/Screen-Shot-2021-03-25-at-2-44-11-PM.png" alt="Screen-Shot-2021-03-25-at-2-44-11-PM" border="0"></a>

 ## what's Telegraf :mailbox_with_mail:

Telegraf is an agent for collecting, processing, aggregating, and writing metrics. :electric_plug:	
Design goals are to have a minimal memory footprint with a plugin system so that developers in the community can easily add support for collecting metrics.
Collect and send all kinds of data:
<br>
Database: Connect to datasources like MongoDB, MySQL, Redis, and others to collect and send metrics.
Systems: Collect metrics from your modern stack of cloud platforms, containers, and orchestrators.
IoT sensors: Collect critical stateful data (pressure levels, temp levels, etc.) from IoT sensors and devices.
