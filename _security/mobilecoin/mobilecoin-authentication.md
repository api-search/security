---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mobilecoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mobilecoin secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mobilecoin
provider_slug: mobilecoin
scheme_count: 1
schemes:
- configured_via: MC_API_KEY environment variable (.env)
  docs: https://mobilecoin.gitbook.io/full-service-api/usage/api-key
  in: header
  name: ApiKeyAuth
  optional: true
  parameter_name: X-API-KEY
  type: apiKey
slug: mobilecoin-authentication
source_filename: mobilecoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mobilecoin.gitbook.io/full-service-api/usage/api-key\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The Full-Service JSON-RPC API runs locally (default 127.0.0.1:9090) and is\n    unauthenticated by default. Optional API-key protection is enabled by\n    setting MC_API_KEY in the service .env; when set, every request must carry\n    the key in the X-API-KEY header. There is no OAuth/OIDC and no scope\n    surface. Network transport can additionally be secured with TLS for the\n    validator and mirror services.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  optional: true\n  configured_via: MC_API_KEY environment variable (.env)\n  docs: https://mobilecoin.gitbook.io/full-service-api/usage/api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobilecoin/refs/heads/main/authentication/mobilecoin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cryptocurrency
- Payments
- Blockchain
- Digital Wallet
- Stablecoins
- Privacy
- JSON-RPC
---
