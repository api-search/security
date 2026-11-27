---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Concessio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Concessio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Concessio
provider_slug: concessio-io
scheme_count: 1
schemes:
- applies_to:
  - rest-api
  - mcp-server
  description: Concessio uses API keys for authentication. Pass your key via the Authorization header. API keys are tied to your organization and plan tier.
  example: 'Authorization: Bearer ck_live_xxxxxxxxxxxx'
  in: header
  issuance: Keys are issued by Concessio to Enterprise customers and approved data partners; there is no self-serve sign-up.
  key_format: ck_live_ followed by 48 hex characters.
  name: Authorization
  scheme: bearer
  type: http
slug: concessio-io-authentication
source_filename: concessio-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://concessio.io/docs/authentication\ndocs: https://concessio.io/docs/authentication\nname: Concessio authentication\nschemes:\n- type: http\n  scheme: bearer\n  name: Authorization\n  in: header\n  description: \"Concessio uses API keys for authentication. Pass your key via the Authorization header. API keys are tied to your organization and plan tier.\"\n  example: \"Authorization: Bearer ck_live_xxxxxxxxxxxx\"\n  key_format: \"ck_live_ followed by 48 hex characters.\"\n  issuance: \"Keys are issued by Concessio to Enterprise customers and approved data partners; there is no self-serve sign-up.\"\n  applies_to: [rest-api, mcp-server]\nunauthenticated_operations:\n- path: /api/v1/id/{CCID}\n  note: \"The public per-ID lookup ( /api/v1/id/ {CCID} ) needs no key; every other endpoint does.\"\n  source: https://concessio.io/docs/api-reference\nmcp: \"The MCP server uses the same key.\"\n"
source_yaml_url: https://artifacts.apis.io/concessio-io/authentication/concessio-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Infrastructure
- Concessions
- Investment Intelligence
- Financial Data
- Project Finance
- MCP
---
