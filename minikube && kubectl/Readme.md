### MINIKUBE COAMMANDS

### To start a cluster:-

```
minikube start
```

### To Access the Kubernetes Dashboard:-

```
minikube dashboard
```

### To Update our cluster:-
```
minikube start --kubernetes-version=latest
```
### Start a second local cluster:-

```
minikube start -p cluster2
```
### To Stop A local Cluster:-

```
minikube stop
```
### To Delete a local cluster:-

```
minikube delete
```

### To Delete all local clusters and profiles:-

```
minikube delete --all
```

### To Allocate memory And Cpu's:-

```
minikube start --cpus 4 --memory 8192
```

### For Allocating VM Driver, container, showing logs, cpu's and memory:-

```
minikube start --vm-driver=xhyve --container-runtime=docker --show-libmachine-logs --v=10 --alsologtostderr --cpus 4 --memory 8192
```

### To get information regarding where your Kubernetes master is running at, CoreDNS is running at, kubernetes-dasboard is running at, we use:-

```
kubectl cluster-info
```

### To get detailed information to further debug and diagnose cluster problem, we use :-

```
kubectl cluster-info dump
```

### To get only the health status for your node we use:-


```kubectl get componentstatus``` or ```kubectl get cs```

### To show detailed information about a resource we use:-


```kubectl describe node <node>```

