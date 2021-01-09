# k8s_study
Truy cập vào từng container trong pod
```
kubectl exec -it <pod-name> bash -c <container-name>
```
Bật proxy trong kubernetes 
```
kubectl proxy --address 0.0.0.0 --accept-hosts '.*'
```
Truy cập vào container thuộc 1 pod nào đó
```
kubectl exec -it <pod-name> -c <container-name> -- bash
```
Sửa thông tin của 1 resource đang chạy
```
kubectl edit -it <resource-kind>/<resource-name>
```
