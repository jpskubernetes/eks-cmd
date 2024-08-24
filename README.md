# EKS (Elastic Kubernetes Service)

`eksctl` is a powerful CLI tool for managing Amazon EKS (Elastic Kubernetes Service) clusters. 

It simplifies the process of creating, managing, and deleting EKS clusters and their associated resources.

## Create a Cluster

```sh
eksctl create cluster \
  --name my-cluster \
  --region us-west-2 \
  --nodes 3 \
  --nodes-min 1 \
  --nodes-max 4 \
  --managed
```
Here’s what each option does:

- `--name my-cluster`: Name of the cluster.
--region us-west-2: AWS region where the cluster will be created.

- `--nodes 3`: Initial number of nodes in the node group.

- `--nodes-min 1`: Minimum number of nodes in the node group.

- `--nodes-max 4`: Maximum number of nodes in the node group.

- `--managed`: Use managed node groups (you can omit this if you want unmanaged nodes).