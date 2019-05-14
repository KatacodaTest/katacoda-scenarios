## Deploy Edge Node

Modify the $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json file. 
Change metadata.name to name of the edge node that you wish to deploy.

`vim $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json`{{execute HOST2 }}

Deploy node using the below command.

_kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/node.json -s cloudhuburl:8080_

Replace clouhuburl with the ip of the machine where your cloud is running(use ens3 iner addr).

Perform above two steps multiple times to create multiple nodes.

You will get a message telling node created.

Pull docker image of edgecore(The image used for this tutorial is created from release version v0.3.0-beta.0).

`docker pull kubeedge/edgecore:v0.3.0-beta.0`{{execute HOST2}}

Tag the image to kubeedge/edgecore:latest.
`docker tag kubeedge/edgecore:v0.3.0-beta.0 kubeedge/edgecore:latest`{{execute HOST2}}