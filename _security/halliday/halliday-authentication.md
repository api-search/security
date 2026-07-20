---
api_key_in: []
api_specs:
- filename: halliday-openapi-original.yml
  format: yaml
  label: Halliday API V2
  slug: halliday-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halliday/refs/heads/main/openapi/halliday-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Halliday Authentication
name_suffix: Authentication
oauth_flows: []
overview: Halliday secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Halliday
provider_slug: halliday
scheme_count: 1
schemes:
- bearerFormat: API_KEY
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/halliday-openapi-original.yml
  type: http
slug: halliday-authentication
source_filename: halliday-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/halliday-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API_KEY\n  sources:\n  - openapi/halliday-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halliday/refs/heads/main/authentication/halliday-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Cryptocurrency
- Blockchain
- Web3
- Onramp
- Swaps
- DeFi
- Agentic Workflows
- Fintech
---
