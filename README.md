# Grafana-EKS

Follow the steps to deploy the Grafana and prometheus
Follow the commands from file helm_deploy-grafana-prom-cmd.txt exactly


Check if all resources created are running.

then create the ingress using command: kubectl apply -f grafana-ingress.yaml

Now you can access the grafana using alb dns
