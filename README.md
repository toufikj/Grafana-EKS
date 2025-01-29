# Grafana-EKS Deployment Guide

This repository provides a comprehensive guide to deploying Grafana and Prometheus on an Amazon EKS cluster using Helm.

## Prerequisites

- **Amazon EKS Cluster**: Ensure you have an operational EKS cluster.
- **Kubernetes CLI (`kubectl`)**: Installed and configured to interact with your EKS cluster.
- **Helm**: Installed on your local machine.

## Deployment Steps

### 1. Clone the Repository

```bash
git clone https://github.com/toufikj/Grafana-EKS.git
cd Grafana-EKS


Follow the steps to deploy the Grafana and prometheus
Follow the commands from file helm_deploy-grafana-prom-cmd.txt exactly

If the pvc is pending state, delete the pending pvc and try again.

Check if all resources created are running.

then create the ingress using command: kubectl apply -f grafana-ingress.yaml

Now you can access the grafana using alb dns

After login to grafana, create a prometheus datasource and add this url: http://prometheus-server.prometheus.svc.cluster.local:80
