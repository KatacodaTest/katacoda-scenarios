# Check Status

This step helps you to check the status of edge node.

Open a new terminal by clicking on + near to current terminal.

Set GOPATH for this terminal.

`export GOPATH=/root/kubeedge`{{execute}}

Now you have both your cloud and edge parts running, 
you can use below command to check the edge node status.

`kubectl get nodes`{{execute}}

####### _If you are getting messages like "No resources found" or any error in connection to server, please re-execute the above step utill you are able to see master node as well as the edge node created._