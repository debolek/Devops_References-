 KUBERNETES ARCHITECTURE 
 
 Kubernetes clusters consist of a set of nodes 
 Nodes :- A node is a physical machine or a virtual on which a kubernetes software set of tools are installed.
 ![image](https://user-images.githubusercontent.com/37187773/139559555-3b70a068-e105-433a-9499-b90e6bcc91d1.png)
 
 A node is a worker machine and that is where container will be lunched by kubernetes 
![image](https://user-images.githubusercontent.com/37187773/139560062-17748e31-fd42-4f9d-bfdd-3bd28cd09ea3.png)

What if the node which the application which is running fails? well obviously,our application goes down . So you need to have more than one nodes so this is where cluster comes in. 

A cluster :- is a set of nodes grouped together this why, even if one nodes fails, you have your application still accessible from the other nodes.
![image](https://user-images.githubusercontent.com/37187773/139560182-b65f23d2-a989-4e28-af21-0aaffa300ede.png)
