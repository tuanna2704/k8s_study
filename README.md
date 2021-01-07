# k8s_study
Truy cập vào từng container trong pod
```
kubectl exec -it <pod-name> bash -c <container-name>
```
Bật proxy trong kubernetes 
```
kubectl proxy --address 0.0.0.0 --accept-hosts '.*'
```
