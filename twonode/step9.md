# Run edge nodes inside containers

Go to the below mentioned path.

`cd $GOPATH/src/github.com/kubeedge/kubeedge/build/edge`{{execute HOST2}}

_./run_daemon.sh only_run_edge mqtt=0.0.0.0:1883 cloudhub=0.0.0.0:10000 edgename=node image="kubeedge/edgecore:latest" containername=container_
 
 Use the above command to deploy your edge node inside container.
 
 _Replace 0.0.0.0 in cloudhub with the ip of the machine where your cloudhub is running._
 
_Replace node with name of node you created._
 
_Replace conatiner with name of container you would like to have._
 
_Repeat this step for multiple nodes. While repeating the same step for next node._
 
 Check Status
 
 `kubectl get nodes`{{execute}}
 
 You can now see your edge nodes in ready state.
