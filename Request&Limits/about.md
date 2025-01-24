Kubernetes requests and limits define the amount of CPU and memory that pod and containers able to consume.


Unexpected resources consumption is one of the most serious challenge that kubernetes adminitrators encounter. This oftern
  has unintended consequences for neighboring pods-if memory capacity is exceeded, then the operating system out-of-memory (oom)
    killer whill intervene by terminating pods.


  $$$$$$$

  kubernetes requests specify the minimum amount of a resources (CPU or memory) that  a pod require to run. 

  This information is used by the kubernetes scheduler to determine which node in the cluster the pod should be palced on.


  Pods that declare a resources request will only schedule to nodes that can provide the requested quantity of the resources.
  This is determined by calculating the sum of the existing requests made by the pods already running on each node.


  ############

  Setting up kubernetes limits:


  A limit is a second kind of constraint that prevents pods from using more than a specified amount of a resources. 
  Whereas requests manages workload-level contention and quality of service, limits are a device for maintaining cluster stability.

  
