# Fullcycle course challenge 

## How to execute

## Requirements

- Docker

- Kubernetes

If you want to execute the services in you machine you to have the **minikube** installed 

### nginx 

```bash
$ cd nginx 
$ kubectl apply -f deployment.yaml 
$ kubectl apply -f service.yaml

# list the services
$ kubectl get svc 

# see the result in your browser
$ minikube service __SERVICE_NAME__
```

### mysql
```bash 
cd mysql
$ kubectl apply -f presistent-volume.yaml
$ kubectl apply -f deployment.yaml 
$ kubectl apply -f service.yaml
```

### greeting 

```bash 
cd greeting
$ kubectl apply -f deployment.yaml 
$ kubectl apply -f service.yaml
```

[Docker Hub Image](https://hub.docker.com/repository/docker/dexfs/go-greeting)

[Github Repository](https://github.com/dexfs/go-greeting)