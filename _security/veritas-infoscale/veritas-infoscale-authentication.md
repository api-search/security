---
api_key_in: []
api_specs:
- filename: veritas-infoscale-rest-api.yaml
  format: yaml
  label: Veritas InfoScale REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-rest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Veritas Infoscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veritas InfoScale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication for InfoScale REST API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/veritas-infoscale-rest-api.yaml
  type: http
slug: veritas-infoscale-authentication
source_filename: veritas-infoscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veritas-infoscale-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication for InfoScale REST API\n  sources:\n  - openapi/veritas-infoscale-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/authentication/veritas-infoscale-authentication.yml
summary_line: http · 1 scheme
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
---
