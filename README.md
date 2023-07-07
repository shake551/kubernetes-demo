# kubernetes-demo
## Installation
```
$ git clone git@github.com:shake551/kubernetes-demo.git
```

## Demo
```
$ cd kubernetes-demo
$ docker build -t python-local-k8s .
# tag local image
$ docker tag python-local-k8s shake551/python-local-k8s
# if you use minikube, you cannot use your local image
# kubectl running on minikube, but your local image is not exist on minikube
$ docker push shake551/python-local-k8s
$ kubectl apply -f manifests/manifest.yml
$ curl localhost:8700
```
