---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dynamic Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dynamic
provider_slug: dynamic-xyz
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dynamic-xyz-openapi.yml
  type: http
slug: dynamic-xyz-authentication
source_filename: dynamic-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dynamic-xyz-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dynamic-xyz-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-xyz/refs/heads/main/authentication/dynamic-xyz-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- Wallets
- Authentication
- Embedded Wallets
- MPC
---
