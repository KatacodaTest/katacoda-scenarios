# Run edge nodes inside containers

Go to the below mentioned path.

`cd $GOPATH/src/github.com/kubeedge/kubeedge/build/edge`{{execute HOST2}}

./run_daemon.sh only_run_edge mqtt=0.0.0.0:1883 cloudhub=0.0.0.0:10000 edgename=node image="kubeedge/edgecore:latest"
 
 Use the above command to deploy your edge node inside container 
 Replace 0.0.0.0 in cloudhub with the ip of the machine where your cloudhub is running
 Also replace node with name of node you created
 
 Repeat this step for multiple nodes. While repeating the same step for next node,
 change the container name from edgecore to any new name in run_daemon.sh(Line No 167)
 
 Check Status
 
 `kubectl get nodes`{{execute HOST1}}
 
 You can now see your edge nodes in ready state.
