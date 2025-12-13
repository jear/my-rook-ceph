# my-rook-ceph

```
helm repo add rook-release https://charts.rook.io/release
helm install --create-namespace --namespace rook-ceph rook-ceph rook-release/rook-ceph 
# helm install --create-namespace --namespace rook-ceph rook-ceph rook-release/rook-ceph -f values.yaml

https://rook.io/docs/rook/v1.12/Getting-Started/example-configurations/#cluster-crd

k apply -f cluster-test.yaml 

https://rook.io/docs/rook/v1.12/Troubleshooting/ceph-toolbox/#interactive-toolbox

k apply -f storageclass-test.yaml 

# Cephfs
k apply -f cephfs-storageclass.yaml
k apply -f filesystem.yaml

# Dashboard
# admin user
kubectl -n rook-ceph get secret rook-ceph-dashboard-password -o jsonpath="{['data']['password']}" | base64 --decode && echo

kubectl proxy
# open http://localhost:8001/api/v1/namespaces/rook-ceph/services/https:rook-ceph-mgr-dashboard:https-dashboard/proxy/ in the browser.

# Toolbox
https://rook-io.netlify.app/docs/rook/v1.2/ceph-toolbox

# Object storage
https://rook-io.netlify.app/docs/rook/v1.2/ceph-object

```
