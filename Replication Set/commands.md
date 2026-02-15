To scale the pods using command alone without editing the replicaset file
kubectl scale rs new-replica-set --replicas=5

Or edit the rs fiel usign edit command and increase the replica to 5
kubectl edit replicaset new-replica-set


Command without editing the yamk file in exam use below command

kubectl create -f /root/deployment-definition-1.yaml --dry-run=client -o yaml | sed 's/kind: deployment/kind: Deployment/' | kubectl apply -f -

**kubectl create -f**: Reads the YAML file to generate a resource.
**--dry-run=client**: Simulates creation locally without actually creating the resource.
**-o yaml**: Outputs the resource definition in YAML format.
Next:

**| sed 's/kind: deployment/kind: Deployment/'**

**|: Pipes the YAML output from the previous command into sed.**
sed 's/kind: deployment/kind: Deployment/': Replaces the lowercase deployment with the correct Deployment (capital D) in the kind field.
Finally:

**| kubectl apply -f -**

|: Pipes the corrected YAML into kubectl apply.
kubectl apply -f -: Applies the resource from standard input (-), effectively creating or updating the deployment with the corrected kind.
In essence, this command creates a corrected deployment manifest on the fly and applies it, fixing the kind issue without editing the original file!
