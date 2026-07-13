---
api_key_in:
- header
api_specs:
- filename: netbird-openapi.yml
  format: yaml
  label: NetBird
  slug: netbird
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbird/refs/heads/main/openapi/netbird-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Netbird Authentication
name_suffix: Authentication
oauth_flows: []
overview: NetBird secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NetBird
provider_slug: netbird
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/netbird-openapi.yml
  type: http
- description: Enter the token with the `Token` prefix, e.g. "Token nbp_F3f0d.....".
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/netbird-openapi.yml
  type: apiKey
slug: netbird-authentication
source_filename: netbird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/netbird-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/netbird-openapi.yml\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Enter the token with the `Token` prefix, e.g. \"Token nbp_F3f0d.....\".\n  sources:\n  - openapi/netbird-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbird/refs/heads/main/authentication/netbird-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Networking
- VPN
- Zero Trust
- Open Source
- WireGuard
- Security
---
