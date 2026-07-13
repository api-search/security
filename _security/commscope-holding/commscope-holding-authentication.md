---
api_key_in: []
api_specs:
- filename: ruckus-one-api-openapi.yml
  format: yaml
  label: RUCKUS One API
  slug: ruckus-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commscope-holding/refs/heads/main/openapi/ruckus-one-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Commscope Holding Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommScope Holding secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CommScope Holding
provider_slug: commscope-holding
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ruckus-one-api-openapi.yml
  type: http
slug: commscope-holding-authentication
source_filename: commscope-holding-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ruckus-one-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ruckus-one-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commscope-holding/refs/heads/main/authentication/commscope-holding-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Points
- Cabling
- Connectivity
- ICX Switches
- Infrastructure
- Networking
- RUCKUS
- Wi-Fi
- Fortune 1000
---
