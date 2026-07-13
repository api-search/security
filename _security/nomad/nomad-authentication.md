---
api_key_in:
- header
api_specs:
- filename: nomad-http-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-http-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nomad Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Nomad secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HashiCorp Nomad
provider_slug: nomad
scheme_count: 2
schemes:
- description: ACL token passed via the X-Nomad-Token request header.
  in: header
  name: nomadToken
  parameter: X-Nomad-Token
  sources:
  - openapi/nomad-http-api-openapi.yml
  type: apiKey
- description: ACL token passed via the Authorization header with Bearer scheme.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nomad-http-api-openapi.yml
  type: http
slug: nomad-authentication
source_filename: nomad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nomad-http-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: nomadToken\n  type: apiKey\n  in: header\n  parameter: X-Nomad-Token\n  description: ACL token passed via the X-Nomad-Token request header.\n  sources:\n  - openapi/nomad-http-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: ACL token passed via the Authorization header with Bearer scheme.\n  sources:\n  - openapi/nomad-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/authentication/nomad-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Workload Orchestration
- Container Orchestration
- Scheduling
- Infrastructure
- DevOps
---
