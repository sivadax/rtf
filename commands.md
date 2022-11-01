**Get all Nodes in K8 Cluster**

`kubectl get node `

**Get all pods running in a K8 Cluster**

`kubectl get pods --all-namespaces`

**Get list of Pods running in a Single Node**
*Replace the IP Address with the node name or node ipadress from the command above*

`kubectl get pods --all-namespaces -o wide --field-selector spec.nodeName=192.168.1.20`

**List all namespaces in K8 Cluster**

`kubectl get namespace `

**Get pod details with ipaddress of all pods**

`kubectl get pods -o wide --all-namespaces`

**Get pod details with ipaddress of all pods in one name space like kube-system**

`kubectl get pods -n kube-system -o wide`

**Watch all pods in K8 cluster**

`watch -n 1 kubectl get pods --all-namespaces`

**Delete a Name Space**

`kubectl delete ns mynamespace`

**Create a Name Space**

`kubectl create ns mynamespace`

**Get logs from a single running pod**

kubectl logs dns-app-install-37508f-fhmgl -n kube-system




