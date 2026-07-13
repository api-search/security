---
api_key_in: []
api_specs:
- filename: rancher-management-api-openapi.yml
  format: yaml
  label: Rancher Management API
  slug: rancher-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/openapi/rancher-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rancher Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rancher secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rancher
provider_slug: rancher
scheme_count: 1
schemes:
- bearerFormat: token-XXXXX:secret
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rancher-management-api-openapi.yml
  type: http
slug: rancher-authentication
source_filename: rancher-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rancher-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token-XXXXX:secret\n  sources:\n  - openapi/rancher-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/authentication/rancher-authentication.yml
summary_line: http · 1 scheme
tags:
- Cluster Management
- Containers
- Kubernetes
- Multi-Cluster
- Open Source
- SUSE
- Platform Engineering
---
