---
anonymous_access: false
api_key_in: []
auth_types:
- delegated-kubernetes-rbac
- registry-credentials
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Carvel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carvel secures its APIs with delegated-kubernetes-rbac and registry-credentials across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Carvel
provider_slug: carvel
scheme_count: 3
schemes:
- applies_to:
  - kapp
  - kctrl
  - kapp-controller
  - secretgen-controller
  detail:
  - App and PackageInstall carry spec.serviceAccountName — kapp-controller impersonates that ServiceAccount for every fetch, template and deploy step, so a package can never exceed the permissions granted to it.
  - spec.cluster.kubeconfigSecretRef lets an App target a different cluster with a kubeconfig held in a Secret.
  - kapp explicitly supports running without admin privileges in a single namespace and creates no CRDs of its own.
  docs: https://carvel.dev/kapp-controller/docs/v0.57.x/security-model/
  name: kubernetes-rbac
  summary: kapp and kctrl act as the current kubeconfig context; the controllers act as the ServiceAccount named in the custom resource. Authorization is Kubernetes RBAC end to end.
  type: delegated
- applies_to:
  - imgpkg
  - kbld
  - vendir
  - kapp-controller
  detail:
  - IMGPKG_REGISTRY_HOSTNAME supports glob wildcards; a non-glob hostname wins over a glob one.
  - In-cluster, kapp-controller reads registry credentials from Kubernetes Secrets, and secretgen-controller's SecretExport/SecretImport pair is the supported way to share one placeholder registry Secret across namespaces.
  docs: https://carvel.dev/imgpkg/docs/v0.46.x/auth/
  name: registry-credentials
  precedence:
  - Environment variables (IMGPKG_REGISTRY_HOSTNAME / _USERNAME / _PASSWORD, indexed and glob-capable since v0.18.0)
  - IaaS-provided credentials (gcr.io, AWS ECR)
  - Command flags
  - Docker config (~/.docker/config.json)
  summary: OCI registry credentials, resolved in a documented precedence order.
  type: delegated
- applies_to:
  - vendir
  - kapp-controller
  docs: https://carvel.dev/vendir/docs/v0.46.x/
  name: git-and-http-source-credentials
  summary: vendir fetches from git, hg, http, githubRelease, helmChart and OCI sources; credentials for those come from the caller's environment or, in-cluster, from a referenced Secret.
  type: delegated
slug: carvel-authentication
source_filename: carvel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://carvel.dev/imgpkg/docs/v0.46.x/auth/ and https://carvel.dev/kapp-controller/docs/v0.57.x/security-model/\ndocs: https://carvel.dev/imgpkg/docs/v0.46.x/auth/\nnote: >-\n  derive-authentication.py found no securitySchemes because there is no OpenAPI to read. Carvel\n  issues no credential of its own; it borrows two credential systems it does not own. Written from\n  the provider's own auth documentation, not inferred.\nsummary:\n  types: [delegated-kubernetes-rbac, registry-credentials]\n  api_key_in: []\n  oauth2_flows: []\n  carvel_issued_credentials: false\nschemes:\n  - name: kubernetes-rbac\n    type: delegated\n    applies_to: [kapp, kctrl, kapp-controller, secretgen-controller]\n    summary: >-\n      kapp and kctrl act as the current kubeconfig context; the controllers act as the\n      ServiceAccount named in the custom resource. Authorization is Kubernetes RBAC end to end.\n    detail:\n      - >-\n        App\
  \ and PackageInstall carry spec.serviceAccountName — kapp-controller impersonates that\n        ServiceAccount for every fetch, template and deploy step, so a package can never exceed the\n        permissions granted to it.\n      - >-\n        spec.cluster.kubeconfigSecretRef lets an App target a different cluster with a kubeconfig\n        held in a Secret.\n      - >-\n        kapp explicitly supports running without admin privileges in a single namespace and creates\n        no CRDs of its own.\n    docs: https://carvel.dev/kapp-controller/docs/v0.57.x/security-model/\n  - name: registry-credentials\n    type: delegated\n    applies_to: [imgpkg, kbld, vendir, kapp-controller]\n    summary: OCI registry credentials, resolved in a documented precedence order.\n    precedence:\n      - Environment variables (IMGPKG_REGISTRY_HOSTNAME / _USERNAME / _PASSWORD, indexed and glob-capable since v0.18.0)\n      - IaaS-provided credentials (gcr.io, AWS ECR)\n      - Command flags\n      - Docker\
  \ config (~/.docker/config.json)\n    detail:\n      - IMGPKG_REGISTRY_HOSTNAME supports glob wildcards; a non-glob hostname wins over a glob one.\n      - >-\n        In-cluster, kapp-controller reads registry credentials from Kubernetes Secrets, and\n        secretgen-controller's SecretExport/SecretImport pair is the supported way to share one\n        placeholder registry Secret across namespaces.\n    docs: https://carvel.dev/imgpkg/docs/v0.46.x/auth/\n  - name: git-and-http-source-credentials\n    type: delegated\n    applies_to: [vendir, kapp-controller]\n    summary: >-\n      vendir fetches from git, hg, http, githubRelease, helmChart and OCI sources; credentials for\n      those come from the caller's environment or, in-cluster, from a referenced Secret.\n    docs: https://carvel.dev/vendir/docs/v0.46.x/\nsupply_chain_verification:\n  cosign: true\n  note: >-\n    Release checksums files are cosign-signed and every release body publishes the verification\n    steps — the closest\
  \ thing Carvel has to an authentication surface it controls itself.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carvel/refs/heads/main/authentication/carvel-authentication.yml
summary_line: delegated-kubernetes-rbac/registry-credentials · 3 schemes
tags:
- CLI
- Configuration
- Containers
- Deployment
- GitOps
- Kubernetes
- Package Management
- Templating
---
