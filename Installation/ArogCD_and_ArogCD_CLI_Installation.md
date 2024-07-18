
# Installation of Argo CD and Argo CD CLI

This guide will outline the steps to install Argo CD on a Kubernetes cluster and set up the Argo CD CLI on your local machine. Argo CD is a declarative, GitOps continuous delivery tool for Kubernetes.

## Create Argo CD Namespace

```bash
kubectl create namespace argocd
```

This command creates a dedicated namespace in your Kubernetes cluster for Argo CD.

## Install Argo CD

```bash
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
kubectl get all --namespace=argocd
```
