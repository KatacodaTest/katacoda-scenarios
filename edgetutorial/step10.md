# Deploy Application

This step helps you to try out a sample application deployment.

`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/deployment.yaml`{{execute}}

Then you can use below command to check if the application is normally running.

`kubectl get pods`{{execute}}