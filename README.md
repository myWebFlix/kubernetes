## ETCD Server

Console access:

```bash
kubectl exec --stdin --tty POD_NAME -- /bin/bash
```

Setting config values:

```bash
kubectl exec --stdin --tty POD_NAME -- etcdctl --endpoints http://0.0.0.0:2379 set /environments/dev/services/webflix-service/1.0.0/config/rest-config/maintenance-mode true
```
