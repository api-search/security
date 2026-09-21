---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: coinrailz-com-agent-payment-api-openapi.yml
  format: yaml
  label: Coin Railz Agent Payment API
  slug: agent-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinrailz-com/refs/heads/main/openapi/coinrailz-com-agent-payment-api-openapi.yml
- filename: coinrailz-com-x402-services-openapi.yml
  format: yaml
  label: Coin Railz x402 Micropayment Services
  slug: x402-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinrailz-com/refs/heads/main/openapi/coinrailz-com-x402-services-openapi.yml
auth_types:
- apiKey
- http
description: Four schemes derived from the Agent Payment API OpenAPI and confirmed against the provider's live machine-readable auth document GET https://coinrailz.com/api/auth/capabilities (HTTP 200, saved verbatim alongside). The x402 services OpenAPI declares no securitySchemes at all; the overlay in overlays/ adds the two that apply. No OAuth2 / OIDC anywhere (well-known metadata 404), so scopes/ is deliberately absent.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Coinrailz Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coin Railz secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coin Railz
provider_slug: coinrailz-com
scheme_count: 4
schemes:
- description: Prepaid credits API key (cr_live_...). Obtain via GET /api/m2m/credits/trial (free $5) or POST /api/m2m/credits/checkout/session (paid).
  in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/coinrailz-com-agent-payment-api-openapi.yml
  type: apiKey
- description: 'Same cr_live_ key as X-API-KEY, passed as Authorization: Bearer <key>.'
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/coinrailz-com-agent-payment-api-openapi.yml
  type: http
- description: x402 protocol on-chain USDC payment. Base64url-encoded signed payment payload. See /.well-known/x402.json for facilitator details.
  in: header
  name: x402
  parameter: X-PAYMENT
  sources:
  - openapi/coinrailz-com-agent-payment-api-openapi.yml
  type: apiKey
- description: 'MPP (Machine Payments Protocol) credential. Authorization: Payment <base64-credential>. See /.well-known/mpp.json.'
  name: mpp
  scheme: payment
  sources:
  - openapi/coinrailz-com-agent-payment-api-openapi.yml
  type: http
slug: coinrailz-com-authentication
source_filename: coinrailz-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/coinrailz-com-agent-payment-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Prepaid credits API key (cr_live_...). Obtain via GET /api/m2m/credits/trial (free $5) or POST /api/m2m/credits/checkout/session\n    (paid).\n  sources:\n  - openapi/coinrailz-com-agent-payment-api-openapi.yml\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: 'Same cr_live_ key as X-API-KEY, passed as Authorization: Bearer <key>.'\n  sources:\n  - openapi/coinrailz-com-agent-payment-api-openapi.yml\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: x402 protocol on-chain USDC payment. Base64url-encoded signed payment payload. See /.well-known/x402.json\n    for facilitator details.\n  sources:\n  - openapi/coinrailz-com-agent-payment-api-openapi.yml\n- name:\
  \ mpp\n  type: http\n  scheme: payment\n  description: 'MPP (Machine Payments Protocol) credential. Authorization: Payment <base64-credential>. See /.well-known/mpp.json.'\n  sources:\n  - openapi/coinrailz-com-agent-payment-api-openapi.yml\ndocs: https://coinrailz.com/api/auth/capabilities\ndocs_file: authentication/coinrailz-com-auth-capabilities.json\ndescription: Four schemes derived from the Agent Payment API OpenAPI and confirmed against the provider's live machine-readable\n  auth document GET https://coinrailz.com/api/auth/capabilities (HTTP 200, saved verbatim alongside). The x402 services\n  OpenAPI declares no securitySchemes at all; the overlay in overlays/ adds the two that apply. No OAuth2 / OIDC\n  anywhere (well-known metadata 404), so scopes/ is deliberately absent.\nauth_modes_published:\n- mode: api_key\n  header: X-API-KEY\n  alternative_header: 'Authorization: Bearer <key>'\n  description: Prepaid credits — fastest path. Works with any HTTP client. No wallet required.\n\
  - mode: x402_onchain\n  header: X-PAYMENT\n  alternative_header: null\n  description: On-chain USDC per-call payments using HTTP 402 protocol. No API key required.\nkey_prefix: cr_live_\nobtain:\n  free_trial: GET https://coinrailz.com/api/m2m/credits/trial ($5, 1 per IP per 7 days, key returned once)\n  hosted_checkout: POST https://coinrailz.com/api/m2m/credits/checkout/session -> Stripe checkoutUrl + retrievalToken\n  direct_card: POST https://coinrailz.com/api/m2m/credits/purchase {paymentMethodId, amountUsd, idempotencyKey}\n  on_chain: answer the 402 challenge with X-PAYMENT (x402 v2, CDP facilitator)\n  mpp: 'Authorization: Payment <credential> per /.well-known/mpp.json'\npublic_operations: 21\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinrailz-com/refs/heads/main/authentication/coinrailz-com-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Payments
- Agents
- x402
- Micropayments
- Cryptocurrency
- DeFi
- Blockchain
- Stablecoins
- USDC
- Prediction Markets
- Satellite Data
- IoT
- Trading
- Compliance
- MCP
- A2A
---
