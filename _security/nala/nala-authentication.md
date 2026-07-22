---
api_key_in:
- header
api_specs:
- filename: nala-rafiki-openapi.yml
  format: yaml
  label: Rafiki API
  slug: rafiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nala/refs/heads/main/openapi/nala-rafiki-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nala Authentication
name_suffix: Authentication
oauth_flows: []
overview: NALA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NALA
provider_slug: nala
scheme_count: 1
schemes:
- expiry: optional (min 180 days)
  format: Bearer {apikey}
  header: Authorization
  in: header
  key_format: xxx.xxx.xxx
  name: bearerApiKey
  provisioning: Rafiki web portal (Settings > API keys)
  scheme: bearer
  scoped: true
  sources:
  - docs.rafiki.com/reference/authentication
  type: http
slug: nala-authentication
source_filename: nala-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.rafiki.com/reference/authentication.md\ndocs: https://docs.rafiki.com/reference/authentication\napi: Rafiki API\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Rafiki authenticates every request with an API key presented as an HTTP\n    Bearer token in the Authorization header. Keys are minted in the Rafiki web\n    portal, are scoped (fine-grained permissions per key), and can carry an\n    optional expiry (minimum TTL 180 days). Key values are shown once and never\n    stored by Rafiki. Key format is a three-part dotted token (xxx.xxx.xxx).\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer {apikey}'\n    key_format: xxx.xxx.xxx\n    scoped: true\n    expiry: optional (min 180 days)\n    provisioning: Rafiki web portal (Settings > API keys)\n    sources: [docs.rafiki.com/reference/authentication]\n\
  scopes_summary:\n  model: per-key scopes (not OAuth2 flows); scopes are selected at key creation\n  scopes:\n    - bank:read\n    - lookup:read\n    - payment-account:read\n    - payment-account:write\n    - payout:read\n    - payout:write\n    - wallet:read\n    - statement:read\n    - statement:write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nala/refs/heads/main/authentication/nala-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Remittances
- Money Transfer
- Payouts
- Cross-Border Payments
- Mobile Money
- Stablecoins
- Africa
---
