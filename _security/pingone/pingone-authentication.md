---
api_key_in: []
api_specs:
- filename: pingone-openapi.yml
  format: yaml
  label: PingOne Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingone/refs/heads/main/openapi/pingone-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pingone Authentication
name_suffix: Authentication
oauth_flows: []
overview: PingOne secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PingOne
provider_slug: pingone
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 Bearer access token issued by the PingOne authentication

    service at auth.pingone.com.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pingone-openapi.yml
  type: http
slug: pingone-authentication
source_filename: pingone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pingone-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 Bearer access token issued by the PingOne authentication\n    service at auth.pingone.com.\n  sources:\n  - openapi/pingone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pingone/refs/heads/main/authentication/pingone-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Authentication
- Authorization
- Single Sign-On
- Multi-Factor Authentication
- IAM
- CIAM
---
