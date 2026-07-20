---
api_key_in:
- header
api_specs:
- filename: bitwise-openapi.yml
  format: yaml
  label: Bitwise API
  slug: bitwise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwise/refs/heads/main/openapi/bitwise-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bitwise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitwise secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitwise
provider_slug: bitwise
scheme_count: 1
schemes:
- description: API key sent in the Authorization header. Request a key from api@bitwiseinvestments.com.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/bitwise-openapi.yml
  type: apiKey
slug: bitwise-authentication
source_filename: bitwise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/bitwise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key sent in the Authorization header. Request a key from api@bitwiseinvestments.com.\n  sources:\n  - openapi/bitwise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitwise/refs/heads/main/authentication/bitwise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Cryptocurrency
- Asset Management
- Market Data
- Index Funds
- ETFs
- Financial Services
---
