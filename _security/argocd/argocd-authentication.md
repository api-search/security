---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: argocd-accountservice-api-openapi.yml
  format: yaml
  label: Argo CD AccountService API
  slug: argocd-accountservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-accountservice-api-openapi.yml
- filename: argocd-applicationservice-api-openapi.yml
  format: yaml
  label: Argo CD ApplicationService API
  slug: argocd-applicationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-applicationservice-api-openapi.yml
- filename: argocd-applicationsetservice-api-openapi.yml
  format: yaml
  label: Argo CD ApplicationSetService API
  slug: argocd-applicationsetservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-applicationsetservice-api-openapi.yml
- filename: argocd-certificateservice-api-openapi.yml
  format: yaml
  label: Argo CD CertificateService API
  slug: argocd-certificateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-certificateservice-api-openapi.yml
- filename: argocd-clusterservice-api-openapi.yml
  format: yaml
  label: Argo CD ClusterService API
  slug: argocd-clusterservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-clusterservice-api-openapi.yml
- filename: argocd-gpgkeyservice-api-openapi.yml
  format: yaml
  label: Argo CD GPGKeyService API
  slug: argocd-gpgkeyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-gpgkeyservice-api-openapi.yml
- filename: argocd-notificationservice-api-openapi.yml
  format: yaml
  label: Argo CD NotificationService API
  slug: argocd-notificationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-notificationservice-api-openapi.yml
- filename: argocd-projectservice-api-openapi.yml
  format: yaml
  label: Argo CD ProjectService API
  slug: argocd-projectservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-projectservice-api-openapi.yml
- filename: argocd-repocredsservice-api-openapi.yml
  format: yaml
  label: Argo CD RepoCredsService API
  slug: argocd-repocredsservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-repocredsservice-api-openapi.yml
- filename: argocd-repositoryservice-api-openapi.yml
  format: yaml
  label: Argo CD RepositoryService API
  slug: argocd-repositoryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-repositoryservice-api-openapi.yml
- filename: argocd-sessionservice-api-openapi.yml
  format: yaml
  label: Argo CD SessionService API
  slug: argocd-sessionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-sessionservice-api-openapi.yml
- filename: argocd-settingsservice-api-openapi.yml
  format: yaml
  label: Argo CD SettingsService API
  slug: argocd-settingsservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-settingsservice-api-openapi.yml
- filename: argocd-versionservice-api-openapi.yml
  format: yaml
  label: Argo CD VersionService API
  slug: argocd-versionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-versionservice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Argocd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argo CD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argo CD
provider_slug: argocd
scheme_count: 1
schemes:
- description: 'JWT Bearer token. Format: Bearer <token>'
  in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/argo-cd-openapi.json
  type: apiKey
slug: argocd-authentication
source_filename: argocd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argo-cd-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Bearer token. Format: Bearer <token>'\n  sources:\n  - openapi/argo-cd-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/authentication/argocd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DevOps
- GitOps
- Kubernetes
- Continuous Delivery
- CNCF
- Open-Source
- Operator
---
