#Deploy Apps

This step helps you to try out a sample application deployment.

Go to this path to see a sample deployment file.

`cd $GOPATH/src/github.com/kubeedge/kubeedge/build`{{execute HOST2}}

`ls`{{execute HOST2}}

You can add a Node Selector in this deployment yaml to schedule the application to a particular edge node.

Then you can use below command to check if the application is normally running.

`kubectl get pods`{{execute}}