---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Murex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Murex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Murex
provider_slug: murex
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token for MX.3 API access
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/murex-market-data-openapi.yml
  - openapi/murex-position-openapi.yml
  - openapi/murex-post-trade-openapi.yml
  - openapi/murex-risk-openapi.yml
  - openapi/murex-trading-openapi.yml
  type: http
slug: murex-authentication
source_filename: murex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/murex-market-data-openapi.yml, openapi/murex-position-openapi.yml, openapi/murex-post-trade-openapi.yml,\n  openapi/murex-risk-openapi.yml, openapi/murex-trading-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token for MX.3 API access\n  sources:\n  - openapi/murex-market-data-openapi.yml\n  - openapi/murex-position-openapi.yml\n  - openapi/murex-post-trade-openapi.yml\n  - openapi/murex-risk-openapi.yml\n  - openapi/murex-trading-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/murex/refs/heads/main/authentication/murex-authentication.yml
summary_line: http · 1 scheme
tags:
- Capital Markets
- Enterprise Software
- Financial Services
- Fintech
- Risk Management
- Trading
---
