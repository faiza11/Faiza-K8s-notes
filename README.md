# Faiza-K8s-notes
These notes will track the progress of kubernetes learnings
Let's learb about Kubernetes services.

Kubernetes undoubtedly provides auto healing capabilities, but let's see what will happen if services are not deployed in kubernetes.
   When a POD goes down, the replica set creates new pods but with a different IP address but other teams may not be aware of this IP address change.  Hence they will not be able to access the application.  To solve this problem a service is created on top of deployment which will help access the pods without IP address.  Services this job by using labels and selectors.

Advantages of services in K8s.
1. Load balancing
2. Service Discovery
3. Expose to outside world

Three types of services implementation
1. Cluster IP - (PODs created using this can only be accessed by the Devoops engineer)
2. Node port implementation - (PODs here can be accessed only by people who has access to the nodes, specifically by people within the organisation)
3. Load balancer - (PODs can be accessed by the outside world)

   
