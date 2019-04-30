# Deploy Edge Node

This step deploys the edge node.

Open a new terminal by clicking on + next to existing terminal.

Set your GOPATH for this terminal

`export GOPATH=/root/kubeedge`{{execute}}

Modify the $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json file. 
Change metadata.name to name of the edge node that you wish to deploy.

`vim $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute}}

Deploy node

`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute}}

If you have changed the path of generated certificates,
then update that path in edge.yaml file present in
$GOPATH/src/github.com/edge/conf/edge.yaml.
If you have not changed the path of certificates, ignore this step.
