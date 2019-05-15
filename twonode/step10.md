# Deploy Apps on edge nodes

This step helps to try out a sample application deployment.

Go to this path to see a sample deployment file.

`cd $GOPATH/src/github.com/kubeedge/kubeedge/build`{{execute HOST2}}

`ls`{{execute HOST2}}

Add a Node Selector in this deployment yaml if you would like to schedule the application to a particular edge node.

_kubectl apply -f deployment.yaml -s cloudhuburl:8080_

Replace cloud hub url with ip of machine where cloud is running.

You can also create your own application and deploy it to edge nodes you create.

Use below command to check if the application is successfully deployed.

`kubectl get pods`{{execute}}

Execute above command untill the application status is "Running".
