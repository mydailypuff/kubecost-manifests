# kubecost-manifests

Kubecost manifest files is created to monitor and manage Kubernetes spends.

Changed the manifests while fixing permission issues in prometheus and kube-state-metrics.

You can access the prometheus with the below command
```
kubectl port-forward --namespace kubecost deployment/kubecost-prometheus-server 9090
```
or with the below url
```
<cluster-dns>/prometheus/graph
```

You can access kubecost with the below command
```
kubectl port-forward -n kubecost service/kubecost 9090:9090
```
or with the below url
```
<cluster-dns>/kubecost/overview
```

## References

https://github.com/kubecost/cost-analyzer-helm-chart/blob/develop/kubecost.yaml
