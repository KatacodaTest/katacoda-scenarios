This step deploys the edge node

`vim $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute}}

Deploy node

`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute}}

Specify the path of certificates to be used in edge.yaml
/etc/kubeedge/ca
/etc/kubeedge/certs

`vim $GOPATH/src/github.com/edge/conf/edge.yaml`{{execute}}