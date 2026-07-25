---
api_key_in:
- header
api_specs:
- filename: argo-cd-accountservice-api-openapi.yml
  format: yaml
  label: Argo CD AccountService API
  slug: argo-cd-accountservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-accountservice-api-openapi.yml
- filename: argo-cd-applicationservice-api-openapi.yml
  format: yaml
  label: Argo CD ApplicationService API
  slug: argo-cd-applicationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-applicationservice-api-openapi.yml
- filename: argo-cd-applicationsetservice-api-openapi.yml
  format: yaml
  label: Argo CD ApplicationSetService API
  slug: argo-cd-applicationsetservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-applicationsetservice-api-openapi.yml
- filename: argo-cd-certificateservice-api-openapi.yml
  format: yaml
  label: Argo CD CertificateService API
  slug: argo-cd-certificateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-certificateservice-api-openapi.yml
- filename: argo-cd-clusterservice-api-openapi.yml
  format: yaml
  label: Argo CD ClusterService API
  slug: argo-cd-clusterservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-clusterservice-api-openapi.yml
- filename: argo-cd-gpgkeyservice-api-openapi.yml
  format: yaml
  label: Argo CD GPGKeyService API
  slug: argo-cd-gpgkeyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-gpgkeyservice-api-openapi.yml
- filename: argo-cd-notificationservice-api-openapi.yml
  format: yaml
  label: Argo CD NotificationService API
  slug: argo-cd-notificationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-notificationservice-api-openapi.yml
- filename: argo-cd-projectservice-api-openapi.yml
  format: yaml
  label: Argo CD ProjectService API
  slug: argo-cd-projectservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-projectservice-api-openapi.yml
- filename: argo-cd-repocredsservice-api-openapi.yml
  format: yaml
  label: Argo CD RepoCredsService API
  slug: argo-cd-repocredsservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-repocredsservice-api-openapi.yml
- filename: argo-cd-repositoryservice-api-openapi.yml
  format: yaml
  label: Argo CD RepositoryService API
  slug: argo-cd-repositoryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-repositoryservice-api-openapi.yml
- filename: argo-cd-sessionservice-api-openapi.yml
  format: yaml
  label: Argo CD SessionService API
  slug: argo-cd-sessionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-sessionservice-api-openapi.yml
- filename: argo-cd-settingsservice-api-openapi.yml
  format: yaml
  label: Argo CD SettingsService API
  slug: argo-cd-settingsservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-settingsservice-api-openapi.yml
- filename: argo-cd-versionservice-api-openapi.yml
  format: yaml
  label: Argo CD VersionService API
  slug: argo-cd-versionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-versionservice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Argo Cd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argo CD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argo CD
provider_slug: argo-cd
scheme_count: 1
schemes:
- description: 'JWT Bearer token. Format: Bearer <token>'
  in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/argo-cd-openapi.json
  type: apiKey
slug: argo-cd-authentication
source_filename: argo-cd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argo-cd-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Bearer token. Format: Bearer <token>'\n  sources:\n  - openapi/argo-cd-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/authentication/argo-cd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
---
