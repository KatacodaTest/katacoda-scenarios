## Check Status

This step helps you to check the status of edge node.

Open a new terminal by clicking on + near to master node.

Set GOPATH for this terminal.

`export GOPATH=/root/kubeedge`{{execute}}
 
You can use below command to check the edge node status.

`kubectl get nodes`{{execute}}

You can see your master(Ready) and edge nodes(Not Ready)
 