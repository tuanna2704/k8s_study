# k8s_study
truy cập vào từng container trong pod
```
kubectl exec -it <pod-name> bash -c <container-name>
```
bật proxy trong kubernetes 
```
kubectl proxy --address 0.0.0.0 --accept-hosts '.*'
```
