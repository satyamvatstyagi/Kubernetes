# Kubernetes Configuration

This repository contains Kubernetes configuration files for deploying a Postgres database and a Go API.

## Postgres

The Postgres configuration includes the following resources:

- ConfigMap: `postgres-config`
- Secret: `postgres-secrets`
- Service: `postgres-headless`
- PersistentVolume: `postgres-pv`
- PersistentVolumeClaim: `postgres-pvc`
- StatefulSet: `postgres`

## Go API

The Go API configuration includes the following resources:

- ConfigMap: `api-config` (in the `development` namespace)
- Secret: `api-secrets` (in the `development` namespace)
- Deployment: `go-api-deployment` (in the `development` namespace)
- HorizontalPodAutoscaler: `go-api-hpa` (in the `development` namespace)
- Service: `go-api-loadbalancer` (in the `development` namespace)
- Ingress: `go-api-ingress` (in the `development` namespace)

For more details on each resource, please refer to the individual YAML files in this repository.
