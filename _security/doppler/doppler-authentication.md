---
api_key_in: []
api_specs:
- filename: doppler-openapi.yml
  format: yaml
  label: Doppler REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppler/refs/heads/main/openapi/doppler-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Doppler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doppler secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Doppler
provider_slug: doppler
scheme_count: 1
schemes:
- bearerFormat: Doppler API Token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/doppler-openapi.yml
  type: http
slug: doppler-authentication
source_filename: doppler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/doppler-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Doppler API Token\n  sources:\n  - openapi/doppler-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doppler/refs/heads/main/authentication/doppler-authentication.yml
summary_line: http · 1 scheme
tags:
- Secrets Management
- SecretOps
- DevOps
- Configuration Management
- Security
- CI/CD
---
