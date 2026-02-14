# Kubernetes
prep for CKA

****Cluster ARchitecture**
1) Master Nodes:
      Manage ,plan schedule and monitor Nodes
2)Worker Nodes:
     Host application as containers.
3) etcd cluster:
      Stores data about diff nodes in a key value format
4) Kube scheduler:

5) Node Controller:
    responsible for creating new nodes
6) Replication Controller:
    Takes care desried number of controllers are runnign at all times
7) Kube api server:
     Which manages all communication between different components .. It exposes Kubernetes API to users who do management operations
   
Consider each container as a ship then kubelet will act as a captain of the ship.. Which reeceives info from Kube api server and acts accordingly like create/destroy containers on nodes.

Both Master nodes and Worker nodes communicates via Kube proxy that ensures neccessary rules are in place.
<img width="978" height="570" alt="image" src="https://github.com/user-attachments/assets/4eb29411-3818-4018-9bf8-4bd3b4fc611f" />


   
