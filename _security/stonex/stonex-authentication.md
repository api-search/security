---
api_key_in: []
api_specs:
- filename: stonex-payments-openapi.yml
  format: yaml
  label: StoneX Payments API
  slug: stonex-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-payments-openapi.yml
- filename: stonex-clearing-openapi.yml
  format: yaml
  label: StoneX Clearing API
  slug: stonex-clearing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-clearing-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stonex Authentication
name_suffix: Authentication
oauth_flows: []
overview: StoneX secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StoneX
provider_slug: stonex
scheme_count: 1
schemes:
- description: JWT token from /auth/token endpoint. Valid for 10 hours.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stonex-clearing-openapi.yml
  - openapi/stonex-payments-openapi.yml
  type: http
slug: stonex-authentication
source_filename: stonex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stonex-clearing-openapi.yml, openapi/stonex-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: JWT token from /auth/token endpoint. Valid for 10 hours.\n  sources:\n  - openapi/stonex-clearing-openapi.yml\n  - openapi/stonex-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/authentication/stonex-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Financial Services
- Payments
- Clearing
- Futures
- Trading
- Risk Management
---
