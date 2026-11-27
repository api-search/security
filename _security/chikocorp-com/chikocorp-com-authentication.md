---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: chikocorp-com-batch-api-openapi.yml
  format: yaml
  label: ChikoCorp Batch API
  slug: chikocorp-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-batch-api-openapi.yml
- filename: chikocorp-com-batches-api-openapi.yml
  format: yaml
  label: ChikoCorp Batches API
  slug: chikocorp-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-batches-api-openapi.yml
- filename: chikocorp-com-cases-api-openapi.yml
  format: yaml
  label: ChikoCorp Cases API
  slug: chikocorp-com-cases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-cases-api-openapi.yml
- filename: chikocorp-com-credits-api-openapi.yml
  format: yaml
  label: ChikoCorp Credits API
  slug: chikocorp-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-credits-api-openapi.yml
- filename: chikocorp-com-preflight-api-openapi.yml
  format: yaml
  label: ChikoCorp Preflight API
  slug: chikocorp-com-preflight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-preflight-api-openapi.yml
- filename: chikocorp-com-reports-api-openapi.yml
  format: yaml
  label: ChikoCorp Reports API
  slug: chikocorp-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-reports-api-openapi.yml
- filename: chikocorp-com-screen-api-openapi.yml
  format: yaml
  label: ChikoCorp Screen API
  slug: chikocorp-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-screen-api-openapi.yml
- filename: chikocorp-com-verification-api-openapi.yml
  format: yaml
  label: ChikoCorp Verification API
  slug: chikocorp-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-verification-api-openapi.yml
- filename: chikocorp-com-watchlist-api-openapi.yml
  format: yaml
  label: ChikoCorp Watchlist API
  slug: chikocorp-com-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-watchlist-api-openapi.yml
- filename: chikocorp-com-webhooks-api-openapi.yml
  format: yaml
  label: ChikoCorp Webhooks API
  slug: chikocorp-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-webhooks-api-openapi.yml
- filename: chikocorp-com-x402-api-openapi.yml
  format: yaml
  label: ChikoCorp X402 API
  slug: chikocorp-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikocorp-com/openapi/chikocorp-com-x402-api-openapi.yml
auth_types:
- apiKey
- http
- x402
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ChikoCorp Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChikoCorp secures its APIs with apiKey, http, and x402 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ChikoCorp
provider_slug: chikocorp-com
scheme_count: 3
schemes:
- description: Clerk browser session; these /api endpoints use current-user ownership rather than machine API keys.
  in: cookie
  name: browserSession
  parameter: __session
  sources:
  - openapi/chikocorp-com-tron-usdt-risk-openapi.yml
  type: apiKey
- description: 'TRON Checker workspace API key sent as Authorization: Bearer. Docs: "Use a bearer API key with the screen:write scope." Live key prefix shown in the docs example: usk_live_. On x402 Launch Verification, the bearer token is the one returned in the case/monitor receipt.'
  key_prefix_live: usk_live_
  name: bearerApiKey
  scheme: bearer
  scopes_documented:
  - screen:write
  scopes_note: Docs say batch, reports, watchlist and webhooks "Use scoped bearer keys" but name no scope other than screen:write.
  sources:
  - openapi/chikocorp-com-tron-usdt-risk-openapi.yml
  - openapi/chikocorp-com-x402-launch-verification-openapi.yml
  - https://usdt.chikocorp.com/api-docs
  type: http
- description: 'Pay-per-request with no account or key: unpaid request receives HTTP 402 + PAYMENT-REQUIRED header; client retries with PAYMENT-SIGNATURE after authorizing USDC on Base. Used by POST /v1/x402/screen (usdt) and the paid x402 Preflight audit/remediation and Launch Verification routes.'
  name: x402
  quote: 'Auth: none (no Clerk, API key, or prepaid credits)'
  sources:
  - https://usdt.chikocorp.com/llms.txt
  - https://usdt.chikocorp.com/api-docs
  - https://x402.chikocorp.com/llms.txt
  type: x402-payment
slug: chikocorp-com-authentication
source_filename: chikocorp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource:\n- https://usdt.chikocorp.com/api-docs\n- https://usdt.chikocorp.com/llms.txt\n- openapi/chikocorp-com-tron-usdt-risk-openapi.yml\n- openapi/chikocorp-com-x402-launch-verification-openapi.yml\ndocs: https://usdt.chikocorp.com/api-docs\nsummary:\n  types:\n  - apiKey\n  - http\n  - x402\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: browserSession\n  type: apiKey\n  in: cookie\n  parameter: __session\n  description: Clerk browser session; these /api endpoints use current-user ownership rather than machine API keys.\n  sources:\n  - openapi/chikocorp-com-tron-usdt-risk-openapi.yml\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: 'TRON Checker workspace API key sent as Authorization: Bearer. Docs: \"Use a bearer API key with the screen:write\n    scope.\" Live key prefix shown in the docs example: usk_live_. On x402 Launch Verification, the bearer token is the one\n    returned in the case/monitor\
  \ receipt.'\n  key_prefix_live: usk_live_\n  scopes_documented:\n  - screen:write\n  scopes_note: Docs say batch, reports, watchlist and webhooks \"Use scoped bearer keys\" but name no scope other than screen:write.\n  sources:\n  - openapi/chikocorp-com-tron-usdt-risk-openapi.yml\n  - openapi/chikocorp-com-x402-launch-verification-openapi.yml\n  - https://usdt.chikocorp.com/api-docs\n- name: x402\n  type: x402-payment\n  description: 'Pay-per-request with no account or key: unpaid request receives HTTP 402 + PAYMENT-REQUIRED header; client\n    retries with PAYMENT-SIGNATURE after authorizing USDC on Base. Used by POST /v1/x402/screen (usdt) and the paid x402 Preflight\n    audit/remediation and Launch Verification routes.'\n  quote: 'Auth: none (no Clerk, API key, or prepaid credits)'\n  sources:\n  - https://usdt.chikocorp.com/llms.txt\n  - https://usdt.chikocorp.com/api-docs\n  - https://x402.chikocorp.com/llms.txt\n"
source_yaml_url: https://artifacts.apis.io/chikocorp-com/authentication/chikocorp-com-authentication.yml
summary_line: apiKey/http/x402 · 3 schemes
tags:
- Company
- Artificial Intelligence
- Cryptocurrency
- x402
- Payments
- Stablecoins
- TRON
- Risk Screening
- Developer Tools
- Diagnostics
---
