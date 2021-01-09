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
Kiểm tra các lần cập nhật
```
kubectl rollout history deploy/<deploy-name>
```
Xem chi tiết các thay đổi trong lần cập nhật
```
kubectl rollout history deploy/<deploy-name> --revision=<number>
```
Rollback về 1 bản cập nhật nào đó
```
kubectl rollout undo deploy/<deploy-name> --to-revision=<number>
```
Còn nếu muốn quay về bản cập nhật ngay trước đó thì chỉ cần dùng lệnh
```
kubectl rollout undo deploy/<deploy-name>
```
