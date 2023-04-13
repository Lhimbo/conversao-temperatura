# Projeto conversão de temperatura

### Sobre o projeto
O projeto conversão de temperatura é um projeto desenvolvido em NodeJS. O projeto tem como objetivo ser um exemplo para a criação de ambiente com containers usando NodeJS.

### Observações do projeto
A aplicação é exposta usando a porta 8080

---
### Comandos Docker
**Build**
```
$ docker build -t $user/conversao-temperatura:v1.0.1 . -f docker/Dockerfile
```
**Logs**
```
$ docker ps
$ docker logs [container_id]
```
**Run**
```
$ docker run -P 8080 -d $user/conversao-temperatura:v1.0.1
```
---
### Comandos K3d
```
$ k3d cluster create [name] [--no-lb] [--agents n] [--servers n] [--port "host:port@loadbalancer"]
$ k3d cluster ls
$ k3d cluster delete
```
---
### Comandos Kubectl
```
$ kubectl get nodes
$ kubectl port-forward node/name host:port
$ kubectl apply -f kube.yaml
```