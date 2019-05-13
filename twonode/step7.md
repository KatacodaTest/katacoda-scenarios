## Deploy Edge Node

Modify the $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json file. 
Change metadata.name to name of the edge node that you wish to deploy.

`vim $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute HOST2 }}

Deploy node
`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute HOST2}}

Perform above two steps multiple times to create multiple nodes

Pull docker image of edgecore
`docker pull kubeedge/edgecontroller-test:v2.1`{{execute HOST2}}
`docker tag kubeedge/edgecontroller-test:v2.1 kubeedge/edgecore:latest`{{execute HOST2}}