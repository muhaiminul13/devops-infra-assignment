# devops-infra-assignment

This repository contains a DevOps project with:
- Terraform EKS setup
- Kubernetes manifests
- CI/CD workflow (GitHub Actions)
- Monitoring and boilerplate folders

## Architecture Diagram
(Add a diagram image here showing EKS cluster, CI/CD flow, monitoring)

## Setup Instructions
1. Terraform: terraform init && terraform apply
2. Kubernetes: kubectl apply -k kubernetes/overlays/dev
3. Monitoring: kubectl apply -f monitoring/

## Security Measures
- RBAC with app service account
- Network policies for pod isolation
- Secrets management (use SOPS or Kubernetes Secrets)

## CI/CD
- GitHub Actions workflow: ci-cd.yaml
- Deploys app to dev/prod environments

## Demo Credentials
- Prometheus: NodePort 30090
- Grafana: NodePort 30300
