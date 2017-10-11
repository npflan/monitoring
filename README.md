# Monitoring

### Quickstart

Deploy Grafana.

First deploy an iSCSI Persistent Volume and then you can deploy grafana with helm.

``` shell
kubectl apply -f extra-pv.yml
helm install -f grafana.vals.yml -n v1 --namespace monitoring stable/grafana
```

