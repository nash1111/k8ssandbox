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
```


参考　　
[GKE k8s](https://cloud.google.com/kubernetes-engine/docs/troubleshooting?hl=ja#connection_refused)