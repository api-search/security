---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gpucloud-ca-api-keys-api-openapi.yml
  format: yaml
  label: GPU Cloud API Keys API
  slug: gpucloud-ca-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-api-keys-api-openapi.yml
- filename: gpucloud-ca-backups-api-openapi.yml
  format: yaml
  label: GPU Cloud Backups API
  slug: gpucloud-ca-backups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-backups-api-openapi.yml
- filename: gpucloud-ca-firewall-api-openapi.yml
  format: yaml
  label: GPU Cloud Firewall API
  slug: gpucloud-ca-firewall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-firewall-api-openapi.yml
- filename: gpucloud-ca-gpu-plans-api-openapi.yml
  format: yaml
  label: GPU Cloud GPU Plans API
  slug: gpucloud-ca-gpu-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-gpu-plans-api-openapi.yml
- filename: gpucloud-ca-metrics-api-openapi.yml
  format: yaml
  label: GPU Cloud Metrics API
  slug: gpucloud-ca-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-metrics-api-openapi.yml
- filename: gpucloud-ca-reservations-api-openapi.yml
  format: yaml
  label: GPU Cloud Reservations API
  slug: gpucloud-ca-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-reservations-api-openapi.yml
- filename: gpucloud-ca-servers-api-openapi.yml
  format: yaml
  label: GPU Cloud Servers API
  slug: gpucloud-ca-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-servers-api-openapi.yml
- filename: gpucloud-ca-ssh-keys-api-openapi.yml
  format: yaml
  label: GPU Cloud SSH Keys API
  slug: gpucloud-ca-ssh-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpucloud-ca/openapi/gpucloud-ca-ssh-keys-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GPU Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: GPU Cloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GPU Cloud
provider_slug: gpucloud-ca
scheme_count: 1
schemes:
- description: 'REST API key (prefix gpu_) created in the GPU Cloud console (Settings). Pass it as `Authorization: Bearer <your-api-key>`. Keys expire after 90 days; a read-only key may only call GET. Write requests (POST, PUT, DELETE) must also send `Origin: https://gpucloud.ca`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/gpucloud-ca-openapi.json
  type: http
slug: gpucloud-ca-authentication
source_filename: gpucloud-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/gpucloud-ca-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'REST API key (prefix gpu_) created in the GPU Cloud console (Settings). Pass\n    it as `Authorization: Bearer <your-api-key>`. Keys expire after 90 days; a read-only key\n    may only call GET. Write requests (POST, PUT, DELETE) must also send `Origin: https://gpucloud.ca`.'\n  sources:\n  - openapi/gpucloud-ca-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gpucloud-ca/authentication/gpucloud-ca-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- GPU
- Compute
- Canada
- Artificial Intelligence
---
