---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Idle Finance API
  slug: idle-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idle/refs/heads/main/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Idle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Idle Finance secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Idle Finance
provider_slug: idle
scheme_count: 1
schemes:
- description: 'Bearer token obtained via https://idlefinance.typeform.com/to/CzRkDH. Include as "Authorization: Bearer <token>" on all requests.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: idle-authentication
source_filename: idle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token obtained via https://idlefinance.typeform.com/to/CzRkDH. Include\n    as \"Authorization: Bearer <token>\" on all requests.'\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idle/refs/heads/main/authentication/idle-authentication.yml
summary_line: http · 1 scheme
tags:
- DeFi
- Yield Optimization
- Finance
- Crypto
- Staking
- Governance
- TVL
- APY
---
