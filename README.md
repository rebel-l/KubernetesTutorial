# KubernetesTutorial
Learning kubernetes ...

Requirements:
- Kubernetes
- Minikube
- Oracle Virtual Box

Start services:

```bash
kubectl create -f .\postgres-deployment.yaml
kubectl create -f .\postgres-service.yaml
kubectl create -f .\webapp-deployment.yaml
kubectl create -f .\webapp-service.yaml
```

Test service:
```bash
curl -v http://$(minikube ip):31317/ping
```

More requests in my Postman `Kubernetes Tutorial`
