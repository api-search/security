---
api_key_in: []
api_specs:
- filename: stablesea-openapi.json
  format: json
  label: Stable Sea Terminal API
  slug: stable-sea-terminal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stablesea/refs/heads/main/openapi/stablesea-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stablesea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stablesea secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stablesea
provider_slug: stablesea
scheme_count: 1
schemes:
- description: Use your API key as the bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/stablesea-openapi.json
  type: http
slug: stablesea-authentication
source_filename: stablesea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/stablesea-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Use your API key as the bearer token\n  sources:\n  - openapi/stablesea-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stablesea/refs/heads/main/authentication/stablesea-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Stablecoins
- Payments
- Cash Management
- Treasury
- Cross-Border Payments
- Liquidity
- Fintech
- On-Off Ramp
- Cryptocurrency
---
