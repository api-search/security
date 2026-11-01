---
anonymous_access: false
api_key_in: []
api_specs:
- filename: circle-audit-logs-api-openapi.yml
  format: yaml
  label: Circle Audit Logs API
  slug: circle-audit-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/circle/openapi/circle-audit-logs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Circle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Circle
provider_slug: circle
scheme_count: 1
schemes:
- description: Circle API key, formatted as `PREFIX:ID:SECRET`, supplied as Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/circle-openapi.yml
  type: http
slug: circle-authentication
source_filename: circle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Circle API key, formatted as `PREFIX:ID:SECRET`, supplied as Bearer token.\n  sources:\n  - openapi/circle-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/circle/authentication/circle-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Compliance
- Cross-Chain
- Currency
- Money
- Payments
- Stablecoins
- Transfers
- USDC
- Wallets
- Stablecoin Issuance
---
