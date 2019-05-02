# Deploy Application

This step helps you to try out a sample application deployment.

`kubectl apply -f $GOPATH/src/github.com/kubeedge/kubeedge/build/deployment.yaml`{{execute}}

Then you can use below command to check if the application is normally running.

`kubectl get pods`{{execute}}

####### _If you are getting messages like "No resources found" or any error in connection to server, please re-execute the above step utill you are able to see the deployment you created._

####### If the STATUS of your deployment is not "Running" please repeat the above step untill it becomes in running status.