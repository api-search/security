---
api_key_in: []
api_specs:
- filename: quantcdn-openapi.yml
  format: yaml
  label: QuantCDN API
  slug: quantcdn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quantcdn/refs/heads/main/openapi/quantcdn-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quantcdn Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuantCDN secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QuantCDN
provider_slug: quantcdn
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Enter your Bearer token in the format: `Bearer <your-token-here>`. Obtain your API token from the QuantCDN dashboard under Profile > API Tokens.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/quantcdn-openapi.yml
  type: http
slug: quantcdn-authentication
source_filename: quantcdn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quantcdn-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Enter your Bearer token in the format: `Bearer <your-token-here>`. Obtain your\n    API token from the QuantCDN dashboard under Profile > API Tokens.'\n  sources:\n  - openapi/quantcdn-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantcdn/refs/heads/main/authentication/quantcdn-authentication.yml
summary_line: http · 1 scheme
tags:
- CDN
- Edge
- Static Hosting
- Jamstack
- DNS
- WAF
- Edge Computing
- Key-Value Storage
- AI Inference
---
