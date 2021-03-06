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
CONTAINER RUNTIME engine like docker  and  
CONTROLLER 

![image](https://user-images.githubusercontent.com/37187773/139560508-f518c68c-30b6-4aad-b2e9-0ebb7ad39e11.png)

API SERVER :- Act like the front end for kubernetes, the users management devices command line interfaces all talk to the API servers to interact with the kubernetes clusters 
ETCD:- Is a key value store used by kubernetes to store all data use to manage a cluster eg if you have a multiple nodes and multiple masters in your cluster etcd stores all the info on all the nodes in your cluster in a distributed manner. NCD is responsible for implmenting a locks within the cluster to ensure there are no conflicts between the masters. 
SCHEDULER :- Responsible for distributing work or containers accross multiple nodes.it looks for newly created containers and assigns them to nodes 
CONTROLLER:- Brain behind orchestration , they are reponsible for noticing and responding when nodes containers or endpoints goes down. The controller makes decisions to bring up new containers. 

CONTAINER RUNTIME :- Is the underlying software that is use to run containers. In our case it happens to be docker 

KUBECTL :- is the agent  responsible for making sure that the cointainers are running on nodes as expected.


Kubectl run hello -minikube
kubectl cluster-info
kubectl get nodes 

Kubectl run my-web-app --image=my-web-app --replicas=100




