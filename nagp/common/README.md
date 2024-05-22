# Kubernetes Configuration

This repository contains Kubernetes configuration files for deploying a Postgres database and a Go API.

## Postgres

The Postgres configuration includes the following resources(in the `development` namespace):

- ConfigMap: `postgres-config`
- Secret: `postgres-secrets`
- Service: `postgres-headless`
- PersistentVolume: `postgres-pv`
- PersistentVolumeClaim: `postgres-pvc`
- StatefulSet: `postgres`

## Go API

The Go API configuration includes the following resources(in the `development` namespace):

- ConfigMap: `api-config`
- Secret: `api-secrets`
- Deployment: `go-api-deployment`
- HorizontalPodAutoscaler: `go-api-hpa`
- Service: `go-api-loadbalancer`
- Ingress: `go-api-ingress`

For more details on each resource, please refer to the individual YAML files in this repository.
