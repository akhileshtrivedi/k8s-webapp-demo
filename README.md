#### Kubernetes files 
* mongo-config.yaml
* mongo-secret.yaml
* mongo-dep-svc.yaml
* webapp-dep-svc.yaml

#### Kubernetes namespaces

There are 3-type of namespace in K8s

1-Default: (Object)-->Pod, Node, Deploy, Svc, config map, etc.

2-kube-public- it is available of everyone.

3-kube-system--Private

##### start Minikube and check status
    brew install minikube
    minikube start --driver docker
    minikube status

##### Here minikube node's ip address
    minikube ip

##### Here basic info about Kubernetes components
    kubectl get node
    kubectl get pod
    kubectl get svc
    kubectl get all

##### Here extended info about components
    kubectl get pod -o wide
    kubectl get node -o wide

##### Here detailed info about a specific component
    kubectl describe service {service-name}
    kubectl describe pod {pod-name}

##### Here application logs
    kubectl logs {pod-name}
    
##### stop your Minikube cluster
    minikube stop

#### Links
* Minikube installation and documentation: https://minikube.sigs.k8s.io/docs/start/
* Kubernetes official documentation: https://kubernetes.io/docs/home/
* Mongodb image on Docker Hub: https://hub.docker.com/_/mongo


