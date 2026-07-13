---
api_key_in: []
api_specs:
- filename: turbonomic-rest-api-openapi.yml
  format: yaml
  label: Turbonomic REST API
  slug: turbonomic-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Turbonomic Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBM Turbonomic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IBM Turbonomic
provider_slug: turbonomic
scheme_count: 1
schemes:
- description: Bearer token obtained by calling POST /api/v3/login with username and password. Include in the Authorization header as 'Bearer {token}'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/turbonomic-rest-api-openapi.yml
  type: http
slug: turbonomic-authentication
source_filename: turbonomic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/turbonomic-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained by calling POST /api/v3/login with username and password.\n    Include in the Authorization header as 'Bearer {token}'.\n  sources:\n  - openapi/turbonomic-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/authentication/turbonomic-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Resource Management
- Cloud Cost Optimization
- Cloud Management
- Hybrid Cloud
- IBM
- Kubernetes
- Multi-Cloud
- Workload Optimization
---
