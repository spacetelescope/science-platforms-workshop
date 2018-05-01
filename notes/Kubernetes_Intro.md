Mathias - NCSA

Intro:
* Started on kubernetes 1.4
* Unstable for a while, 1.8 is trying for backward api compatability
* Kubernetes seems to have overtaken mesos and dockerswarm

Diagram
* Showed the different components of the systems
  - Master(s) / Nodes
  - Masters
    - API server (endpoint)
    - etcd for cluster status (replicated)
    - scheduler maps pods to nodes
    - controller manager: tells scheduler to keep N pods of X type active
  - Nodes
    - Kubelet
    - docker
    - kube-proxy for communication with the apiserver on masters

Concepts:
 - Pod: a group of containers
 - Labels: tagging for pods/services/etc...
 - kubelet: container agent
 - proxy: pod load balancer
 - etcd: metadata service

Diagram 2:
 - Clusters have multiple namespaces
  - Security
  - Encapsulation
 - Ingress exposes service outside the cluster
 - Service exposes container poirt to cluster
 - Pod: Collection of containers

Security:
 - Namespaces partition the cluster
 - Lables select resource within cluster or namespace
 - Can create service accounts with specific roles
 - Roles scoped to namespace
 - Cluster roles are global to the cluster
 - Network policies determine how services can talk to each other and the outside world
 
Resource Manager:
 - Can limit cpu,memory, sotorage within namespace
 - Can limit pod counts per node
 
Went over a few different example k8s diagrams


DesLabs demo:
* Dockerfile
  - Extended nginx:alpine
  - Added a hello stsci index.html
  - Built the demo container
  - Pushed the container to dockerhub
* Conneted to k8s cluster
  - showed kubectl command demos
  - showed deploying the stsci demo docker image using a kubectl config file
    - Added container in config file
    - Added service in config file (for exposing the container port)
    - kubectl apply -f demo.yaml
  - showed creating an ingress controller to expose the service to the outside world
  - showed changing the replicas for redundancy
  - showed updating the base image and deploying it to relevent nodes
  
