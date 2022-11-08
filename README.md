入門 Kubernetesのメモ

```
# login
gcloud auth login
# enable api
gcloud services enable service:container.googleapis.com
# components install
gcloud components install gke-gcloud-auth-plugin
# make cluster
gcloud container clusters create [cluster-name]
# get credentials
gcloud container clusters get-credentials [cluster-name]
# create pods
kubectl apply -f [targetyamlfile]
# delete pods
kubectl delete -f [targetyamlfile]
# exec commands
kubectl exec [pod name] -- [command]
# interactive execution
kubectl exec -it [pod name] -- ash
# file transfer(pod to local)
kubectl [pod name]:[path] [local path]
# file transfer(local to pod)
kubectl [local path] [podname]:[path]
```


参考　　
[GKE k8s](https://cloud.google.com/kubernetes-engine/docs/troubleshooting?hl=ja#connection_refused)