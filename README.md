# ArgoCD GitOps

This repository demonstrates a GitOps workflow using ArgoCD and Kubernetes.

The project manages Kubernetes resources through Git and uses ArgoCD to continuously synchronize cluster state with the desired configuration stored in the repository.

## Overview

The repository contains ArgoCD resources and environment-specific Kubernetes manifests for managing application deployments.

Features include:

- ArgoCD Applications
- ArgoCD Projects
- ArgoCD ApplicationSets
- Automatic Synchronization
- Self-Healing
- Multi-Environment Deployments

## Repository Structure

argocd-gitops

applications/
├── manifests/
├── projects/
└── applicationsets/

environments/
├── dev/
└── prod/

## Environments

### Development

- Kubernetes Namespace
- Deployment
- Service

### Production

- Dedicated Kubernetes manifests
- Replica configuration
- Resource requests and limits

## GitOps Workflow

Git Repository
    │
    ▼
ArgoCD
    │
    ▼
Kubernetes Cluster

Any change committed to Git can be synchronized automatically to the target Kubernetes environment through ArgoCD.

## Technologies Used

- ArgoCD
- Kubernetes
- GitOps
- YAML
- Git
- GitHub

## Key Concepts Demonstrated

- GitOps Deployment Model
- Multi-Environment Configuration
- ApplicationSet Management
- Automated Synchronization
- Self-Healing Applications
- Declarative Kubernetes Deployments

## Future Enhancements

- Helm Integration
- Kustomize Overlays
- Progressive Delivery
- Multi-Cluster Deployments
