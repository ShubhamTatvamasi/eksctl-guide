# eksctl-guide

create an EKS cluster
```bash
eksctl create cluster -f mycluster.yaml
```

get clusters list
```bash
eksctl get cluster
```

scale down cluster to 1 node
```bash
eksctl scale nodegroup --cluster MY-cluster --name ng-1 --nodes-min 1 --nodes 1
```

delete the cluster
```bash
eksctl delete cluster --name MY-cluster
```
---

### AWS Commands

list all clusters
```bash
aws eks list-clusters
```

describe cluster
```bash
aws eks describe-cluster --name cluster_name
```

save config of cluster
```bash
aws eks --region region update-kubeconfig --name cluster_name
```
