# k8s-lab

My first Kubernetes tests, on a single-node k3s cluster
(Ubuntu Server VM on VirtualBox). Lab only, not production.

## Files
- `01_nginx.yml`: nginx Deployment (3 replicas)
- `02_service.yml`: NodePort Service (port 30080) to reach nginx from outside the cluster

## What I did
- Installed k3s
- Deployed nginx from a YAML manifest
- Scaled from 1 to 3 replicas by editing the file and running `kubectl apply`
- Self-healing test: deleted a pod, it was recreated automatically
- Accessed nginx from a Windows PC through the VM's IP (`192.168.1.25:30080`)

## Next
Namespaces, Ingress, persistent volumes.
