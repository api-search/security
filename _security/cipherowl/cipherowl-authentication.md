---
api_key_in: []
api_specs:
- filename: cipherowl-openapi.json
  format: json
  label: CipherOwl SRR API
  slug: cipherowl-srr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cipherowl/refs/heads/main/openapi/cipherowl-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cipherowl Authentication
name_suffix: Authentication
oauth_flows: []
overview: CipherOwl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CipherOwl
provider_slug: cipherowl
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained from /oauth/token using client credentials.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cipherowl-openapi.json
  type: http
slug: cipherowl-authentication
source_filename: cipherowl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cipherowl-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained from /oauth/token using client credentials.\n  sources:\n  - openapi/cipherowl-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cipherowl/refs/heads/main/authentication/cipherowl-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Compliance
- Crypto
- Security
- Risk
- Sanctions Screening
- AML
- Digital Assets
- Stablecoins
- Web3
---
