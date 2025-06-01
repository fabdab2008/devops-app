## Kubernetes Deployment

This app is deployed using a single-node `k0s` Kubernetes cluster.

### Setup k0s cluster

```bash
curl -sSLf https://get.k0s.sh | sudo sh
sudo k0s install controller --single
sudo k0s start
sudo k0s kubeconfig admin > ~/.kube/config
chmod 600 ~/.kube/config
kubectl get nodes

