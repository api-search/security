---
api_key_in: []
api_specs:
- filename: infisical-infisical-api-openapi.yml
  format: yaml
  label: Infisical REST API
  slug: infisical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infisical/refs/heads/main/openapi/infisical-infisical-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Infisical Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infisical secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Infisical
provider_slug: infisical
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: An access token in Infisical
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/infisical-infisical-api-openapi.yml
  type: http
slug: infisical-authentication
source_filename: infisical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/infisical-infisical-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: An access token in Infisical\n  sources:\n  - openapi/infisical-infisical-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infisical/refs/heads/main/authentication/infisical-authentication.yml
summary_line: http · 1 scheme
tags:
- Secrets Management
- Security
- DevOps
- Developer Tools
- Open Source
- PKI
- Certificates
- Privileged Access Management
- CI/CD
- Kubernetes
- Environment Variables
- Encryption
---
