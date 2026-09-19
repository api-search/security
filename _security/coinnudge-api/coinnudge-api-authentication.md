---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'The CoinNudge Data API authenticates every request with a customer-issued API key presented as an HTTP Bearer token. Keys are minted in the private key and download workspace and are scoped to the account''s active plan. There is no OAuth, OpenID Connect, or public no-key tier: even the free Research scope requires a signed-in account key.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coinnudge Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinNudge API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CoinNudge API
provider_slug: coinnudge-api
scheme_count: 1
schemes:
- format: 'Authorization: Bearer <API_KEY>'
  header: Authorization
  key_prefix: cnd_
  notes: A 401 is returned for invalid, missing, or revoked keys. Anonymous probes of both the free Research catalog and the paid Market Events catalog return 401 with detail "Use a customer data Bearer key, not an internal audit token.", confirming the whole surface is key-gated.
  placement: request header only (never in query string or public contexts)
  scheme: bearer
  type: http
slug: coinnudge-api-authentication
source_filename: coinnudge-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://coinnudge.site/data/api-docs\nname: CoinNudge Data API Authentication\ndescription: >-\n  The CoinNudge Data API authenticates every request with a customer-issued API\n  key presented as an HTTP Bearer token. Keys are minted in the private key and\n  download workspace and are scoped to the account's active plan. There is no\n  OAuth, OpenID Connect, or public no-key tier: even the free Research scope\n  requires a signed-in account key.\nschemes:\n  - type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Authorization: Bearer <API_KEY>'\n    key_prefix: cnd_\n    placement: request header only (never in query string or public contexts)\n    notes: >-\n      A 401 is returned for invalid, missing, or revoked keys. Anonymous probes\n      of both the free Research catalog and the paid Market Events catalog return\n      401 with detail \"Use a customer data Bearer key, not an internal audit\n     \
  \ token.\", confirming the whole surface is key-gated.\nkey_management:\n  issued_at: https://coinnudge.site/data/workspace\n  key_slots_by_plan:\n    free: 1 key\n    researcher: 1 key\n    research_desk: up to 5 keys (rate limit shared across the account)\n  slot_exhaustion_status: 409 (all API key slots exhausted)\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinnudge-api/refs/heads/main/authentication/coinnudge-api-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Market Data
- Trading
- Quantitative Finance
- Research
- Derivatives
- Financial Data
- Datasets
---
