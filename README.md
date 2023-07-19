# my-rook-ceph

```
helm repo add rook-release https://charts.rook.io/release
helm install --create-namespace --namespace rook-ceph rook-ceph rook-release/rook-ceph 
# helm install --create-namespace --namespace rook-ceph rook-ceph rook-release/rook-ceph -f values.yaml

https://rook.io/docs/rook/v1.12/Getting-Started/example-configurations/#cluster-crd

k apply -f cluster-test.yaml 

https://rook.io/docs/rook/v1.12/Troubleshooting/ceph-toolbox/#interactive-toolbox

k apply -f storageclass-test.yaml 


```
