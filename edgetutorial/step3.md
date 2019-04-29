RootCA certificate and a cert/key pair is required to have a setup for KubeEdge. Same cert/key pair can be used in both cloud and edge.

`$GOPATH/src/github.com/kubeedge/kubeedge/build/tools/certgen.sh genCertAndKey edge`{{execute}}

The cert/key will be generated in the /etc/kubeedge/ca and /etc/kubeedge/certs respectively.