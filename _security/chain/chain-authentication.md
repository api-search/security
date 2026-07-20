---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Chain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chain
provider_slug: chain
scheme_count: 1
schemes:
- format: Bearer [example key] (live) / Bearer [example key] (sandbox)
  header: Authorization
  in: header
  key_prefixes:
    live: sk_live_
    sandbox: sk_sandbox_
  name: bearerApiKey
  scheme: bearer
  type: http
slug: chain-authentication
source_filename: chain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://chain.com/documentation/authentication\ndocs: https://chain.com/documentation/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: bearer\n  oauth2_flows: []\nnotes: >-\n  Chain uses API-key authentication passed as a Bearer token in the Authorization header. Keys are\n  environment-scoped by prefix: sk_sandbox_ for the testing environment and sk_live_ for production\n  (live keys move real money). No OAuth is documented.\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer [example key] (live) / Bearer [example key] (sandbox)'\n  key_prefixes:\n    live: sk_live_\n    sandbox: sk_sandbox_\nheaders:\n- name: Authorization\n  required: true\n  description: Bearer token containing the API key.\n- name: Content-Type\n  required: true\n  description: Must be application/json for request bodies.\n- name: X-Business-Id\n  required:\
  \ false\n  description: Required when managing multiple businesses under one account.\n- name: X-Idempotency-Key\n  required: false\n  description: Unique key for safe request retries.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chain/refs/heads/main/authentication/chain-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- Stablecoin
- Cryptocurrency
- Blockchain
- Financial Services
- Wallets
- Cards
- Cross-Border Payments
- API
---
