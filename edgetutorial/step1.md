This step basically set up the environment necessary.

make master available on insecure port 8080

`vim /etc/kubernetes/manifests/kube-apiserver.yaml`{{execute}}
Edit - --insecure-port=8080
Add - --insecure-bind-address=0.0.0.0

Initially we can create a folder to which we will be cloning the base code

`mkdir kubeedge`{{execute}}

Switch to the created directory and create the src directory(for GOPATH setting)

`cd kubeedge`{{execute}}

`mkdir src`{{execute}}

Set GOPATH for working

`export GOPATH=/root/kubeedge`{{execute}}

Verify whether your GOPATH is set correctly

`echo $GOPATH`{{execute}}
