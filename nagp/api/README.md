# Kubernetes App

This repository contains the Kubernetes configuration files for deploying the Go API application.

## ConfigMap

The ConfigMap stores configuration values that are used by the application.

## Secret

The Secret stores sensitive data like database credentials and JWT keys in a base64 encoded format.

## Deployment

The Deployment deploys the Go API application with 3 replicas, setting up the necessary environment variables from ConfigMap and Secret. It uses a rolling update strategy for zero-downtime deployments.

## HorizontalPodAutoscaler (HPA)

The HorizontalPodAutoscaler (HPA) automatically scales the number of replicas based on CPU utilization, with a minimum of 1 and a maximum of 5 replicas.

## Service

The Service exposes the Go API application as a LoadBalancer service, making it accessible from outside the cluster.
