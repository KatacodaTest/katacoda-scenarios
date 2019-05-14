# Copy the certificate generated to edge node

Copy the certificates generated in master to the node01 in path /etc/kubeedge/ca and /etc/kubeedge/certs

`cd /etc`{{execute HOST2}}
Create path for copying certificates.
`mkdir kubeedge`{{execute HOST2}}
`cd ca`{{execute HOST2}}
`mkdir ca`{{execute HOST2}}
`mkdir certs`{{execute HOST2}}

Copy the generated certificates.
`scp -r /etc/kubeedge/ca root@node01:/etc/kubeedge`{{execute HOST1}}

`scp -r /etc/kubeedge/certs root@node01:/etc/kubeedge`{{execute HOST1}}

##### _This is the default path. You can keep certificates in any path you like but make sure you give that path for certificates in upcoming steps._