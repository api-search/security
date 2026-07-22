---
api_key_in: []
api_specs:
- filename: obol-openapi-original.json
  format: json
  label: Obol API
  slug: obol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-openapi-original.json
- filename: docs-json
  format: yaml
  label: Obol API OpenAPI (live)
  slug: obol-api-openapi-live
  spec_type: OpenAPI
  url: https://api.obol.tech/docs-json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Obol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Obol secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Obol
provider_slug: obol
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/obol-openapi-original.json
  type: http
slug: obol-authentication
source_filename: obol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/obol-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/obol-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/authentication/obol-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Crypto
- Ethereum
- Staking
- Distributed Validators
- Blockchain Infrastructure
- Web3
---
