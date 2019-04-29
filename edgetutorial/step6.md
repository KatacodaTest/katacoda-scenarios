This step deploys the edge node

`vim $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute}}

Deploy node

`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute}}