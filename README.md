# k8s-deployments

To deploy all applications, simply run

```bash
kubectl apply -f .
```

This installs all ArgoCD Applications.

Your DNS Suffix is `she-test.com`. So to access the URLs add the following entries in your local `/etc/hosts` file

```bash
sudo vi /etc/hosts

172.18.0.6      argocd.she-test.com grafana.she-test.com prometheus.she-test.com opensearch.she-test.com  alertmanager.she-test.com minio.she-test.com
```

The IP Address must match to the External IP Address which is used in the service of your internal_nginx LoadBalancer.

Add new entries to this line accordingly.
