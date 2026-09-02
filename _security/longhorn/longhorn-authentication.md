---
api_key_in: []
api_specs:
- filename: longhorn-backingimages-api-openapi.yml
  format: yaml
  label: Longhorn BackingImages API
  slug: longhorn-backingimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-backingimages-api-openapi.yml
- filename: longhorn-backups-api-openapi.yml
  format: yaml
  label: Longhorn Backups API
  slug: longhorn-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-backups-api-openapi.yml
- filename: longhorn-engineimages-api-openapi.yml
  format: yaml
  label: Longhorn EngineImages API
  slug: longhorn-engineimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-engineimages-api-openapi.yml
- filename: longhorn-nodes-api-openapi.yml
  format: yaml
  label: Longhorn Nodes API
  slug: longhorn-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-nodes-api-openapi.yml
- filename: longhorn-recurringjobs-api-openapi.yml
  format: yaml
  label: Longhorn RecurringJobs API
  slug: longhorn-recurringjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-recurringjobs-api-openapi.yml
- filename: longhorn-settings-api-openapi.yml
  format: yaml
  label: Longhorn Settings API
  slug: longhorn-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-settings-api-openapi.yml
- filename: longhorn-snapshots-api-openapi.yml
  format: yaml
  label: Longhorn Snapshots API
  slug: longhorn-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-snapshots-api-openapi.yml
- filename: longhorn-systembackups-api-openapi.yml
  format: yaml
  label: Longhorn SystemBackups API
  slug: longhorn-systembackups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-systembackups-api-openapi.yml
- filename: longhorn-volumes-api-openapi.yml
  format: yaml
  label: Longhorn Volumes API
  slug: longhorn-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-volumes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Longhorn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Longhorn secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Longhorn
provider_slug: longhorn
scheme_count: 1
schemes:
- description: Kubernetes service account token for authenticating with the Longhorn Manager API. Typically passed via the Kubernetes API proxy.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/longhorn-manager-api-openapi.yml
  type: http
slug: longhorn-authentication
source_filename: longhorn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/longhorn-manager-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Kubernetes service account token for authenticating with the Longhorn Manager\n    API. Typically passed via the Kubernetes API proxy.\n  sources:\n  - openapi/longhorn-manager-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/authentication/longhorn-authentication.yml
summary_line: http · 1 scheme
tags:
- Backup
- Block Storage
- Cloud-Native
- Incubating
- Kubernetes
- PersistentVolumes
---
