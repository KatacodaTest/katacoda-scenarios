## Deploy Edge Node

Modify the $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json file. 
Change metadata.name to name of the edge node that you wish to deploy.

`vim $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute HOST2 }}

Deploy node using the below command.
kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json -s cloudhuburl:8080

Perform above two steps multiple times to create multiple nodes

Pull docker image of edgecore
`docker pull kubeedge/edgecore`{{execute HOST2}}
`docker tag kubeedge/edgecore kubeedge/edgecore:latest`{{execute HOST2}}