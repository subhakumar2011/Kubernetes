**Pod creation Yaml** files had 4 top level elements which are
* apiVersion
* kind
* metadata
* spec
Commands used

kubectl run nginx --image=nginx to create pods
kuebctl get pods
kubectl describe pods <pod-name>
kubectl delete <pod-name>
  
<img width="1386" height="555" alt="image" src="https://github.com/user-attachments/assets/0d6df2ec-50f2-43e8-b334-4cca6dd1ef1f" />

spec is a  had elements in a list/array(It can have info of single container or multi container thats why its list or array)
