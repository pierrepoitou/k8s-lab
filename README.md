# k8s-lab

Mes premiers tests Kubernetes, sur un cluster k3s mono-noeud
(VM Ubuntu Server sous VirtualBox).

## Fichiers
- 01_nginx.yml : Deployment nginx (3 replicas)
- 02_service.yml : Service NodePort (port 30080) pour acceder a nginx hors du cluster

## Ce que j'ai fait
- Installation de k3s
- Deploiement de nginx avec un manifest YAML
- Passage de 1 a 3 replicas en modifiant le fichier puis kubectl apply
- Test d'auto-reparation : suppression d'un pod, recreation automatique
- Acces a nginx depuis un PC Windows via l'IP de la VM contenant le cluster soit 192.168.1.25:30080

## A venir
Namespaces, Ingress, volumes persistants...
