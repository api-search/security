---
api_key_in: []
api_specs:
- filename: onelogin-openapi.yml
  format: yaml
  label: OneLogin API
  slug: onelogin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onelogin/refs/heads/main/openapi/onelogin-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Onelogin Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneLogin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OneLogin
provider_slug: onelogin
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/onelogin-openapi.yml
  type: http
slug: onelogin-authentication
source_filename: onelogin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/onelogin-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/onelogin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onelogin/refs/heads/main/authentication/onelogin-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Access Management
- Single Sign-On
- Multi-Factor Authentication
- SAML
- OAuth
---
