# Helm Helper

During `helm init` Helm does not set up a service account. On Kubernetes deployments with RBAC set up, this results in permissions issues when running commands like `helm list` and `helm install`. This shell script runs the necessary `kubectl` commands to create the service account.
