# lootbot.cloud cluster components
This repository contains the source code for the cluster-security and cluster-management components.

## Components
- [cluster-security](cluster-security/README.md): The cluster security component is responsible for managing the cluster's PodSecurityPolicy and PodSecurtiyAdmissionController resources.
- [flux-system](flux-system/README.md): The flux-system component is responsible for managing the cluster's Flux resources.
- [downstream](downstream/README.md): The downstream component is responsible for managing the cluster's downstream resources.
### Prerequisites
- [Docker](https://www.docker.com/)
- [Kustomize](https://kustomize.io/)
- [Kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)