# k8s



```
kubectl get svc
NAME                                TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)        AGE
kubernetes                          ClusterIP   10.43.0.1      <none>        443/TCP        32m
nestjs-metrics-kube-state-metrics   ClusterIP   10.43.226.33   <none>        8080/TCP       32m
nestjs-metrics-prometheus-server    ClusterIP   10.43.181.61   <none>        80/TCP         32m
nestjs-metrics-grafana              NodePort    10.43.91.163   <none>        80:30694/TCP   32m



Get the key from cluster: kubectl get secret <grafana-secret-name> -o jsonpath="{.data.<secret-key>}" | base64 --decode
```