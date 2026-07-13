---
api_key_in: []
api_specs:
- filename: portworx-openapi.yml
  format: yaml
  label: Portworx
  slug: portworx
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portworx/refs/heads/main/openapi/portworx-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Portworx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Portworx secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Portworx
provider_slug: portworx
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/portworx-openapi.yml
  type: http
slug: portworx-authentication
source_filename: portworx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/portworx-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/portworx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portworx/refs/heads/main/authentication/portworx-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Native
- Containers
- Data Management
- Kubernetes
- Storage
---
