# Run Edge

This step runs the edge.

For running edge, you need to update some parameters in edge.yaml file which are listed below:

1. Replace edgehub.websocket.certfile and edgehub.websocket.keyfile with your own certificate path(if you have changed the certificate path)

2. Replace fb4ebb70-2783-42b8-b3ef-63e2fd6d242eq with edge node name in edge.yaml for the below fields :

   1. websocket:URL
   2. controller:node-id
   3. edged:hostname-override

After making the above mentioned updations, run edge using the command given below:

`./edge_core`{{execute}}
