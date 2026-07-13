---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pinata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinata secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pinata
provider_slug: pinata
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Pinata JWT issued from the Pinata dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pinata-openapi.yml
  type: http
slug: pinata-authentication
source_filename: pinata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pinata-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Pinata JWT issued from the Pinata dashboard.\n  sources:\n  - openapi/pinata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinata/refs/heads/main/authentication/pinata-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- IPFS
- Storage
- Gateway
---
