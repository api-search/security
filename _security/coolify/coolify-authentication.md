---
api_key_in: []
api_specs:
- filename: coolify-openapi.yml
  format: yaml
  label: Coolify
  slug: coolify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-openapi.yml
- filename: coolify-openapi.yml
  format: yaml
  label: Coolify REST API
  slug: coolify-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coolify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coolify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coolify
provider_slug: coolify
scheme_count: 1
schemes:
- description: Go to `Keys & Tokens` / `API tokens` and create a new token. Use the token as the bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/coolify-openapi.yml
  type: http
slug: coolify-authentication
source_filename: coolify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coolify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Go to `Keys & Tokens` / `API tokens` and create a new token. Use the token as\n    the bearer token.\n  sources:\n  - openapi/coolify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/authentication/coolify-authentication.yml
summary_line: http · 1 scheme
tags:
- Platform as a Service
- Self-Hosting
- Deployment
- Open Source
- Containers
- Docker
---
