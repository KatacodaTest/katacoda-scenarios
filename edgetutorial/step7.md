Run Edge

Modify the $GOPATH/src/github.com/kubeedge/kubeedge/edge/conf/edge.yaml configuration file

Replace edgehub.websocket.certfile and edgehub.websocket.keyfile with your own certificate path

Update the IP address of the master in the websocket.url field.

replace fb4ebb70-2783-42b8-b3ef-63e2fd6d242eq with edge node name in edge.yaml for the below fields :

websocket:URL
controller:node-id
edged:hostname-override

After making necessary updations run edge

`./edge_core`{{execute}}
