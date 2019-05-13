#Check Status

`kubectl get nodes`{{execute HOST1}}

#Deploy Apps


This step helps you to try out a sample application deployment.

`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/deployment.yaml`{{execute HOST2}}

Then you can use below command to check if the application is normally running.

`kubectl get pods`{{execute HOST1}}