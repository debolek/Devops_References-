 KUBERNETES ARCHITECTURE 
 
 Kubernetes clusters consist of a set of nodes 
 Nodes :- A node is a physical machine or a virtual on which a kubernetes software set of tools are installed.
 ![image](https://user-images.githubusercontent.com/37187773/139559555-3b70a068-e105-433a-9499-b90e6bcc91d1.png)
 
 A node is a worker machine and that is where container will be lunched by kubernetes 
![image](https://user-images.githubusercontent.com/37187773/139560062-17748e31-fd42-4f9d-bfdd-3bd28cd09ea3.png)

What if the node which the application which is running fails? well obviously,our application goes down . So you need to have more than one nodes so this is where cluster comes in. 

A cluster :- is a set of nodes grouped together this why, even if one nodes fails, you have your application still accessible from the other nodes.
![image](https://user-images.githubusercontent.com/37187773/139560182-b65f23d2-a989-4e28-af21-0aaffa300ede.png)

Now we have a cluster but who is responsible for managing this clusters?where is the information about the number of clusters are stored ?how are the nodes monitored?When the node fails?How do you move the workload of a node to another worker node when it fails, that's where the master comes in

Master :- Is a node with the kubernetes control plane components installed.The master watches over the nodes are in the cluster and is responsible for the actual orechestration of containers on the worker nodes
![image](https://user-images.githubusercontent.com/37187773/139560469-011d9962-4ce0-477d-85c0-640c5e0d350c.png)

When you install a Kubernetes on a system you are actually installing the following components,You are installing the following components:- 

API SERVER,
SCHEDULER,
ETCD,
KUBECTL,
CONTAINER RUN TIME and  
CONTROLLER 

![image](https://user-images.githubusercontent.com/37187773/139560508-f518c68c-30b6-4aad-b2e9-0ebb7ad39e11.png)

