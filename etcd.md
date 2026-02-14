ETCD
etcd is used to store data in key value format. I t stores data aboout the following 
* Nodes
* Pods
* Configs
* Secrets
* Accounts
* Roles
* Bindings
* Other                    

Kube APi server is the central part in Master nodes which takes care of the following (When request hits first it reaches Kube server  only)
* Authenticate User
*Validate Request
* Retrieve Data
* Update ETCD
* SCheduler
* Kubelet
Pod
Pod is a single instance of your application.
pod can have container o fyour application and also it can accomadate a helper container if needed to support your application. So now both containers are in same pod and they share the same network and volumes. they are in one to one relationship.
kubectl run nignix What this command does are below

created a pod automatically
deploys our container in the pod pulls  image from docker hub.



