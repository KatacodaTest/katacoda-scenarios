# Environment Setup

This step basically setup the environment necessary for deploying kubeedge.

Make master available on insecure port 8080 and update insecure bind address to 
0.0.0.0 for edgecontroller/kubectl to work with http connection to Kubernetes apiserver. 
Update this parameters in the kube-apiserver.yaml file.

Edit - --insecure-port=8080

Add - --insecure-bind-address=0.0.0.0

The below command will open the file and update the details in the file as specified.

`vim /etc/kubernetes/manifests/kube-apiserver.yaml`{{execute}}

Create a folder for cloning the base code.

`mkdir kubeedge`{{execute}}

Switch to the created directory and create the src directory(for GOPATH setting)

`cd kubeedge`{{execute}}

`mkdir src`{{execute}}

Set GOPATH

`export GOPATH=/root/kubeedge`{{execute}}

Verify whether your GOPATH is set correctly

`echo $GOPATH`{{execute}}




