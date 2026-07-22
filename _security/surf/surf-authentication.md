---
api_key_in:
- header
api_specs:
- filename: surf-openapi-original.json
  format: json
  label: Surf Data API
  slug: surf-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-openapi-original.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Surf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Surf secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Surf
provider_slug: surf
scheme_count: 3
schemes:
- audience: public
  bearerFormat: JWT
  header: 'Authorization: Bearer sk-...'
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/surf-openapi-original.json
  type: http
- audience: internal
  in: header
  name: AdminToken
  parameter: X-Admin-Token
  sources:
  - openapi/surf-openapi-original.json
  type: apiKey
- audience: internal
  in: header
  name: InternalKey
  parameter: X-Internal-Key
  sources:
  - openapi/surf-openapi-original.json
  type: apiKey
slug: surf-authentication
source_filename: surf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/surf-openapi-original.json\ndocs: https://agents.asksurf.ai/docs/cli/introduction\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  public_scheme: bearer\nnotes: >-\n  Public access uses a single Bearer API key (keys are prefixed `sk-`), passed in the\n  `Authorization: Bearer $SURF_API_KEY` header, generated from the dashboard at\n  agents.asksurf.ai. The OpenAPI also declares AdminToken (X-Admin-Token) and InternalKey\n  (X-Internal-Key) apiKey schemes that are internal/admin-only and not for public consumers.\n  The gateway also serves 30 free credits per day per IP with no key at all.\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  audience: public\n  header: 'Authorization: Bearer sk-...'\n  sources:\n  - openapi/surf-openapi-original.json\n- name: AdminToken\n  type: apiKey\n  in: header\n  parameter: X-Admin-Token\n  audience: internal\n  sources:\n\
  \  - openapi/surf-openapi-original.json\n- name: InternalKey\n  type: apiKey\n  in: header\n  parameter: X-Internal-Key\n  audience: internal\n  sources:\n  - openapi/surf-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/authentication/surf-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Crypto
- Blockchain
- Market Data
- On-Chain Analytics
- Wallet Intelligence
- AI
- DeFi
- Prediction Markets
- Developer API
---
