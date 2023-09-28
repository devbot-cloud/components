# ToDo V1 Milestones (post-beta)
- [ ] Workloads automatically update
- [ ] Helm Charts are able to be pulled from OCI repos
- [ ] Kustomize remote ref is replaced by flux includes
- [ ] Flux is updated to v1 GA
- [ ] Flux is configured to use https over SSH for git repos.
- [ ] Flux sharding is implements on a per cluster basis
- [ ] External secrets is updated to a version supporting push secrets.
    - Retire config syncer
    - Depricate kyverno move namespace policies
- [ ] Refactor infra vars gitrepo
    - Create repos for specific infrastructure implementations/configurations.
- [ ] Replace global vars with vault 
- [ ] Implement flux semver
    - Depricate folder versioning
- [ ] Implement Istio 
    - Ingress Gateway
        - Set istio ingress as default over Nginx
    - Implement MTLS
    - Implement istio JWT keycloak integration
- [ ] Begin planning for air-gapped Gitops-Toolkit implementaitn
    - agtk (airgapped-toolkit)
    - Rough ideas for implementation
    - Roadmap
    - Key goals and milestones for the project.
- [ ] Upgrade kubernetes version from 1.24.7 -> 1.27.x
- [ ] Increase vmlink from 1gbps -> 10gpbs
- [ ] 
# Gitops -> Gitops-Toolkit (Project)
Overarching project containing cluster management 
## Components (Project -> Repo)
Contains the main compoents for cluster creation and management.
- These were split into seperate projects, but may need to rejoined
    - Downstream 
    - Management

### Management (repo -> folder)
Configuration specific to the management clsuters
- flux-system
- workloads
- cluster-security (depricated with k8s 1.25)
### Downstream (repo -> folder)
Configuration specific to the downstream clsuters
- workloads

## Clusters (Project)
Definitions for the clusters, management, and downstream
### Mgmt
### Loot

## Workloads
Defines workloads which are consumed by the management, and downstream clusters.
### Podinfo
### Avi