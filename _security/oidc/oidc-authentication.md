---
api_key_in: []
api_specs:
- filename: oidc.yml
  format: yaml
  label: OpenID Connect API
  slug: openid-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oidc Authentication
name_suffix: Authentication
oauth_flows: []
overview: OIDC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OIDC
provider_slug: oidc
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer Token obtained through OIDC authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oidc.yml
  type: http
slug: oidc-authentication
source_filename: oidc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oidc.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer Token obtained through OIDC authentication.\n  sources:\n  - openapi/oidc.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/authentication/oidc-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity
- JWT
- OAuth
- OIDC
- OpenID Connect
---
