## Deploy Edge Node

Pull docker image
`docker pull lidiya92/edgecore`{{execute HOST2}}
`docker tag lidiya92/edgecore kubeedge/edgecore:latest`{{execute HOST2}}


Modify the $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json file. 
Change metadata.name to name of the edge node that you wish to deploy.

`vim $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute HOST2 }}

Deploy node

`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute HOST2}}
