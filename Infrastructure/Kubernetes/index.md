## Kubernetes
Kubernetes is an opensource platform to orchestate and manage containerize application, this was intially developed by google but now is manteined by the Cloud Native Compute Fundation(CNCF). Kubernete provides a way to automate the deployment, scalability, and management containerize applications running on cloud environments or local datacenters.


Most cotainer orchestrators can:
1. Group hosts: This refers to the ability of K8s to group together physical or virtual hosts to from a cluster, which can be managed as a single entity.

2. Schedule containers based on resources availability: K8s has a built-in scheduler system that can automatically assign containers to available hosts based on resource availability and workload requeriments.

3. Containers communication along of cluster: K8s provides a network overlay that enables containers running on duffenrent hosts to communicate with each other using standard networking protocols, without need for manual configuration.

4. Bind containers with storage resources: K8s offers a mechanism for containers to comsume storage resources such as local disk, network-attach storage(NAS), and cloud-base storage services.

5. Sets of continainers loadbalancing: K8s provides a built-in load balancer that can distribute traffic across multiple containers running the same application, and can also provide an external IP address for accessing the application.

6. Manage and optimize resource usage: K8s includes features for monitoring and optimizing resource usage, such as automatic scaling based on resource utilization, resource quotas, and resources limits.

7. Secure policies for access: K8s provides security features such as network isolation, authentication, and authorization, which can be used to secure access to applications running inside containers. It also supports integration with external security providers such as LDAP or OAuth.

Kubernetes offers a vey rich set of features for container orchestration. Some of its fully supported features are:

* Automatic container packing
Kubernetes automatically schedules containers based on resource needs and contrains, to mazimize utilization without sacrificing availability.

* Designed for extensibility
A Kubernetes cluster can be extended with new custome features without modifying the upstream source code. It use different way to offers this capability such as Custom Resource Definitions (CRDs), Operators, Kubectl plugins, Kubernetes API.

* Self-healing
Kubernetes automatically replace and reschedules containers from failed nodes. It terminates and then restarts containers that become unresponsive to health checks, base on existing rules/policy. It also prevents traffic from being routed to unresponsive containers.

* Horizontal scaling
With kubernetes applications are scaled manually or automatically based on CPU or custom metrics utilization.

* Service discovery and load balancing
Containers recive IP addresses from Kubernetes, while it assigns a single Domain Name System (DNS) name to a set of containers to help in load-balancing request across the containers of the set.

* Automated rollouts and rollbacks
Kubernetes seamlessly rolls out and rolls back application updates and configuration changes, constantly monitoring the application's heath to prevent any downtime.

* Secret and configuration management
Kubernetes manages sensitive data and configuration details for an application separately from the conntainr image, in order to avoid a rebuild of respective image. Secretes consist of sentive/confidential information passed to the application without revealing the sensitive content to the stack configuration, like on GitHub.

* Storage orchestration
Kebernetes automatically mounts software-define storage (SDS) solution to containers fro local storage, external cloud providers, distributed storage or network storage systems.

* Batch execution
Kubernetes support batch execution, long-running jobs, and replaces failed contianers.

* IPv4/IPv6 dual-stack
Kubernetes supports both IPv4 and IPV6 addresses.

There are many addutional features currently in alpha or beta phase. For example, support role-based access control (RBAC) is stable only as of the Kubernetes 1.8 release.
