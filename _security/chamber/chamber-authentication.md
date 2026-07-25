---
api_key_in: []
api_specs:
- filename: chamber-capacity-api-openapi.yml
  format: yaml
  label: Chamber Capacity API
  slug: chamber-capacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-capacity-api-openapi.yml
- filename: chamber-health-api-openapi.yml
  format: yaml
  label: Chamber Health API
  slug: chamber-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-health-api-openapi.yml
- filename: chamber-metrics-api-openapi.yml
  format: yaml
  label: Chamber Metrics API
  slug: chamber-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-metrics-api-openapi.yml
- filename: chamber-workloads-api-openapi.yml
  format: yaml
  label: Chamber Workloads API
  slug: chamber-workloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-workloads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chamber Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chamber secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chamber
provider_slug: chamber
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token — a JWT from Cognito or a Chamber API token (prefix `ch.`). Generate API tokens in the dashboard under Settings > API Tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chamber-openapi.yml
  type: http
slug: chamber-authentication
source_filename: chamber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/chamber-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token — a JWT from Cognito or a Chamber API token (prefix `ch.`). Generate\n    API tokens in the dashboard under Settings > API Tokens.\n  sources:\n  - openapi/chamber-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/authentication/chamber-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU
- AIOps
- Machine Learning
- MLOps
- Infrastructure
- Cloud
- Kubernetes
- Observability
- Monitoring
- Company
---
