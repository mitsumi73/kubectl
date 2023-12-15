# Kết Nối với Cluster
Sau khi cài đặt, bạn cần cấu hình kubectl để kết nối với Kubernetes cluster. Điều này thường được thực hiện bằng cách thiết lập một file cấu hình Kubernetes (thường là ~/.kube/config).

# Các Lệnh Cơ Bản
kubectl get nodes: Liệt kê tất cả các nodes trong cluster.

kubectl get pods: Hiển thị thông tin về tất cả các pods trong namespace hiện tại.

kubectl create -f <file.yaml>: Tạo một tài nguyên (ví dụ: pod, service, deployment, v.v.) từ một file YAML.

kubectl apply -f <file.yaml>: Áp dụng cấu hình từ file YAML lên cluster.

kubectl delete -f <file.yaml>: Xóa tài nguyên được xác định trong file YAML.

kubectl logs <pod-name>: Xem logs từ một pod cụ thể.

# Namespaces
Kubernetes hỗ trợ multiple namespaces để giúp phân chia các tài nguyên giữa các nhóm người dùng và dự án khác nhau. 

Ví dụ, kubectl get pods --namespace <namespace-name> sẽ liệt kê các pods trong một namespace cụ thể.
