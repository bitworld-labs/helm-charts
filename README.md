# BitWorld Helm Charts


This Repository contains all the charts used by BitWorld for different components and is maintained by BitWorld.

## Introduction

Some charts are used by BitOps for its functionality and other charts are also provided which can be used to add additional features and components in BitOps Cluster.

The Charts with its functionality is listed below:

- [Kube Prometheus Stack](https://github.com/prometheus-operator/kube-prometheus) as a end-to-end Kubernetes cluster monitoring with Prometheus
- [Argocd](https://github.com/argoproj/argo-cd/) as a declarative, GitOps CD tool
- [Argo Workflows](https://github.com/argoproj/argo) as a container-native workflow engine for orchestrating parallel jobs on Kubernetes, it works as a CI in BitOps Dashboard
- [Clair](https://github.com/quay/clair) & [Guard](https://github.com/guard/guard) for Image Scanning in application containers
- [Nats Server](https://github.com/nats-io/nats-server) as a High Performance Server for [NATS](https://github.com/nats-io)
- [Nats Streaming](https://github.com/nats-io/k8s) for NATS Streaming Cluster Setup in BitOps
- [Argo Rollout](https://github.com/argoproj/argo-rollouts) used as a K8s controller which provide advanced deployment capabilities such as blue-green, canary, canary analysis, experimentation, and progressive delivery features to Kubernetes
- [Kubewatch](https://github.com/bitnami-labs/kubewatch) a Kubernetes watcher that currently publishes events notifications through webhooks
- [Calico Networking](https://github.com/projectcalico/calico) implements the Kubernetes Container Network Interface (CNI) as a plug-in and provides agents for K8s to provide networking for containers and pods.
- [Dgraph](https://github.com/dgraph-io/charts) as a distributed graph database
- [Coralogix](https://github.com/coralogix/fluentd-coralogix-image) for log collection, real time insights and trend analysis
- [AWS SSM Agent](https://github.com/aws/amazon-ssm-agent) used to install SSM Agent on EKS worker nodes
- [Cluster Essentials](https://github.com/bitworld-labs/charts/tree/main/charts/cluster-essentials) used to install all the infra essentials that a kubernetes cluster needs
- [BitOps Backup](https://github.com/bitworld-labs/charts/tree/main/charts/bitworld-backups) used to take backup of BitOps
- [BitOps Generic Helm](https://github.com/bitworld-labs/charts/tree/main/charts/bitworld-generic-helm) used to deploy any custom YAML file or group of resources
- [BitOps](https://bitworld.solutions/) used to install and configure BitOps
- [BitOps Secrets](https://github.com/bitworld-labs/charts/tree/main/charts/dt-secrets) used to create Secrets in BitOps Cluster
- [GitSensor](https://github.com/bitworld-labs/charts/tree/main/charts/gitsensor) used for BitOps component git-sensor which keeps checking for recent commits on your source code repository
- [Mautic](https://www.mautic.org/) used as a email-marketing tool in K8s Cluster
- [Knative Installer](https://knative.dev/docs/) to enable serverless workloads to run on Kubernetes Cluster
- [Kube State Metric](https://github.com/kubernetes/kube-state-metrics) used to install kube-state-metrics to generate and expose cluster-level metrics
- [Secret Replicator](https://github.com/bitworld-labs/charts/tree/main/charts/secret-replicator) used to create secrets in multiple Namespaces in BitOps Cluster

## How to use the charts

### Install with Helm

These charts are currently not available on the official helm repository therefore you need to download it to install.

```bash
helm repo add bitworld http://bitworld.github.io/helm-charts
helm install Chart-Release-Name bitworld/chartName
```

Each Chart also has a seperate Readme file to understand the usage in BitOps.

## Contributing

