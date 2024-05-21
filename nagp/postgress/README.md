# PostgreSQL Deployment on Kubernetes

This guide explains how to deploy a PostgreSQL database on a Kubernetes cluster using ConfigMap, Secret, Headless Service, PersistentVolume, PersistentVolumeClaim, and StatefulSet.

## Components

### ConfigMap

Contains configuration data for the PostgreSQL database name and user.

### Secret

Contains the PostgreSQL password, encoded in base64.

### Headless Service

A headless service for PostgreSQL, used for DNS-based service discovery.

### PersistentVolume

Defines a persistent volume on the host path for data storage.

### PersistentVolumeClaim

Requests persistent storage for the StatefulSet.

### StatefulSet

Manages the deployment and scaling of PostgreSQL pods with persistent storage. The volumeMounts and volumeClaimTemplates ensure that the database data is persisted.