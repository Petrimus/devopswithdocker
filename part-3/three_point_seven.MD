# Container Orchestration

If you want to run your application you can use Docker to run it. This creates a single instance of your application. 
If you need another one for example, due to heavy traffic to your application, 
you need to run another Docker container and maybe a load balancer in a yet new container in front of application containers.
Also, Docker host that runs containers can crash too, which results in the termination of all containers hosted by it.
When application size gets larger and the number of containers grows, it becomes impractical (or even impossible) to monitor 
and maintain all the needed containers by yourself. 

## Kubernetes
Kubernetes, a container orchestration software, is a solution for previous. It has a set of tools and scripts 
that can help host containers in a production environment. It usually consists of multiple Docker hosts 
that can host containers. It is meant for container deployment operations, scaling up and down, 
and automation across the clusters of hosts.

## Kubernetes vs. Swarm
There are other orchestration tools available besides Kubernetes, which is created by Google. 
A Docker has its own orchestration tool called Swarm. Both of these tools are widely in use. 
Docker Swarm is easy to use and is prefered by developers who prefer fast deployment and simplicity, 
but it lacks some advanced features that Kubernetes have. Kubernetes uses its own YAML, 
which defers from the one Docker uses, whereas Swarm offers much of the familiar functionality from Docker. 
