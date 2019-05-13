# Environment Setup for Edge Nodes

###Install GoLang abd set GOROOT and GOPATH


`wget https://dl.google.com/go/go1.10.3.linux-amd64.tar.gz`{{execute HOST2}}
`sudo tar -xvf go1.10.3.linux-amd64.tar.gz`{{execute HOST2}}
`sudo mv go /usr/local`{{execute HOST2}}
`export GOROOT=/usr/local/go`{{execute HOST2}}

`mkdir kubeedge`{{execute HOST2}}
`cd kubeedge`{{execute HOST2}}

`mkdir src`{{execute HOST2}}
`export GOPATH=/root/kubeedge`{{execute HOST2}}
`export PATH=$GOPATH/bin:$GOROOT/bin:$PATH`{{execute HOST2}}