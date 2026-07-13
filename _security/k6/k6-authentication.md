---
api_key_in: []
api_specs:
- filename: k6-openapi.yml
  format: yaml
  label: K6
  slug: k6
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/k6/refs/heads/main/openapi/k6-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: K6 Authentication
name_suffix: Authentication
oauth_flows: []
overview: K6 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: K6
provider_slug: k6
scheme_count: 1
schemes:
- description: Grafana Cloud k6 API token (Personal or Grafana Stack token) supplied as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/k6-openapi.yml
  type: http
slug: k6-authentication
source_filename: k6-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/k6-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Grafana Cloud k6 API token (Personal or Grafana Stack token) supplied as a Bearer\n    token in the Authorization header.\n  sources:\n  - openapi/k6-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/k6/refs/heads/main/authentication/k6-authentication.yml
summary_line: http · 1 scheme
tags:
- Load Testing
- Testing
---
