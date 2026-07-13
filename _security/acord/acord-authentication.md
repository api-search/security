---
api_key_in: []
api_specs:
- filename: acord-ngds-openapi.yml
  format: yaml
  label: ACORD Next-Generation Digital Standards (NGDS) API
  slug: acord-ngds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/openapi/acord-ngds-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Acord Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ACORD secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ACORD
provider_slug: acord
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://auth.insurer-internal.example.com/oauth/token
  name: oauth2
  sources:
  - openapi/acord-ngds-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/acord-ngds-openapi.yml
  type: http
slug: acord-authentication
source_filename: acord-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acord-ngds-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.insurer-internal.example.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/acord-ngds-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/acord-ngds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/authentication/acord-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
---
