# Run edge nodes as containers


 ./run_daemon.sh only_run_edge mqtt=0.0.0.0:1883 cloudhub=0.0.0.0:10000 edgename=node image="kubeedge/edgecore:latest"
 
 Use the above command to deploy your edge node inside container 
 Replace 0.0.0.0 in cloudhub with the ip of the machine where your cloudhub is running
 Also replace node with name of node you created
 