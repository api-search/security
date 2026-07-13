---
api_key_in: []
api_specs:
- filename: 1password-connect-openapi.yml
  format: yaml
  label: 1Password Connect Server API
  slug: 1password-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-connect-openapi.yml
- filename: 1password-events-openapi.yml
  format: yaml
  label: 1Password Events API
  slug: 1password-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-events-openapi.yml
- filename: 1password-partnership-openapi.yml
  format: yaml
  label: 1Password Partnership API
  slug: 1password-partnership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-partnership-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 1Password Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1Password secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 1Password
provider_slug: 1password
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A Connect server access token generated from 1Password. Each request must include this token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/1password-connect-openapi.yml
  - openapi/1password-events-openapi.yml
  - openapi/1password-partnership-openapi.yml
  type: http
slug: 1password-authentication
source_filename: 1password-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/1password-connect-openapi.yml, openapi/1password-events-openapi.yml, openapi/1password-partnership-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A Connect server access token generated from 1Password. Each request must include\n    this token in the Authorization header.\n  sources:\n  - openapi/1password-connect-openapi.yml\n  - openapi/1password-events-openapi.yml\n  - openapi/1password-partnership-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/authentication/1password-authentication.yml
summary_line: http · 1 scheme
tags:
- Password Manager
- Passwords
- Security
- Secrets
---
