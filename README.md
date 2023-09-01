# nirmata-kube-controller
This repository consists of chart files for nirmata kube controller which is used for connecting your cluster to Nirmata Policy Manager (NPM). 

**Add the nirmata kube controller Helm repository:**

```console
helm repo add nirmata-kube-controller https://nirmata.github.io/nirmata-kube-controller-helm/
helm repo update nirmata-kube-controller
```

Once the repository is added, the cluster can be added to NPM by installing the helm chart.

```console
helm install myNPMcluster nirmata-kube-controller/nirmata-kube-controller. --set cluster.name=mytestcluster --set apiToken="xxxxxxxxxxxxxxxx"
NAME: mycluster
LAST DEPLOYED: Fri Sep  1 00:02:11 2023
NAMESPACE: default
STATUS: deployed
REVISION: 1
TEST SUITE: None

```
