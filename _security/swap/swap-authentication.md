---
api_key_in:
- header
- query
- body
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Swap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swap secures its APIs with apiKey and http across 8 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Swap
provider_slug: swap
scheme_count: 8
schemes:
- additional: 'Authorization: Bearer <ID token> and x-store-id for shopper-facing flows'
  in: header
  name: agentic-storefront-public-key
  parameter: x-public-key
  source: https://docs.api-swap-os.com/quickstart/authentication/
  surface: Agentic Storefront API
  type: apiKey
- name: agentic-storefront-wire-session
  parameter: session id + token from POST /v1/agents/session/authorize
  scheme: bearer
  source: https://docs.api-swap-os.com/products/agentic-storefront/getting-started/authentication/
  surface: Agentic Storefront API (Wire Worker realtime)
  transport: websocket
  type: http
- in: header
  name: global-api-key
  parameter: x-api-key
  source: https://docs.api-swap-os.com/products/global/authentication/
  store_scope: key is store-scoped
  surface: Global API
  type: apiKey
- in: header
  name: protect-api-key
  parameter: x-api-key
  source: https://docs.api-swap-os.com/products/protect/
  surface: Protect API
  type: apiKey
- in: header
  name: returns-api-key-v1
  parameter: X-API-Key
  source: https://docs.api-swap-os.com/products/returns/
  store_parameter: store (query, V1) / store_id (Quality Control, body)
  surface: Returns API (V1) + Quality Control
  type: apiKey
- in: header
  name: returns-api-key-v2
  parameter: X-API-Key
  source: https://docs.api-swap-os.com/products/returns/external-returns/
  store_parameter: swap_store_id (query)
  surface: Returns API (V2)
  type: apiKey
- in: header
  name: shipping-api-key
  parameter: x-api-key
  source: https://docs.api-swap-os.com/products/shipping/environments-and-auth/
  store_parameter: storeId (request body)
  surface: Shipping / Swap Values API
  type: apiKey
- in: header
  name: tlc-api-key
  parameter: x-api-key
  source: https://docs.api-swap-os.com/products/tlc/environments-and-auth/
  surface: TLC API
  type: apiKey
slug: swap-authentication
source_filename: swap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.api-swap-os.com/quickstart/authentication/\ndocs: https://docs.api-swap-os.com/quickstart/authentication/\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query, body]\n  oauth2_flows: []\n  model: >-\n    API keys are issued per-API (surface) and per-environment (a Global key\n    cannot call Returns; a sandbox key cannot call production). Every request is\n    also scoped to a store via a store identifier whose parameter name differs by\n    surface. Shopper-facing Agentic Storefront flows add a bearer ID token.\nnotes:\n  - Header names are case-insensitive; surfaces vary between x-api-key and X-API-Key.\n  - No OAuth2 or OpenID Connect; this is a key-auth platform, so there is no scope surface.\nschemes:\n  - name: agentic-storefront-public-key\n    surface: Agentic Storefront API\n    type: apiKey\n    in: header\n    parameter: x-public-key\n    additional: 'Authorization: Bearer <ID token> and\
  \ x-store-id for shopper-facing flows'\n    source: https://docs.api-swap-os.com/quickstart/authentication/\n  - name: agentic-storefront-wire-session\n    surface: Agentic Storefront API (Wire Worker realtime)\n    type: http\n    scheme: bearer\n    parameter: 'session id + token from POST /v1/agents/session/authorize'\n    transport: websocket\n    source: https://docs.api-swap-os.com/products/agentic-storefront/getting-started/authentication/\n  - name: global-api-key\n    surface: Global API\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    store_scope: key is store-scoped\n    source: https://docs.api-swap-os.com/products/global/authentication/\n  - name: protect-api-key\n    surface: Protect API\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    source: https://docs.api-swap-os.com/products/protect/\n  - name: returns-api-key-v1\n    surface: Returns API (V1) + Quality Control\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    store_parameter:\
  \ 'store (query, V1) / store_id (Quality Control, body)'\n    source: https://docs.api-swap-os.com/products/returns/\n  - name: returns-api-key-v2\n    surface: Returns API (V2)\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    store_parameter: 'swap_store_id (query)'\n    source: https://docs.api-swap-os.com/products/returns/external-returns/\n  - name: shipping-api-key\n    surface: Shipping / Swap Values API\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    store_parameter: 'storeId (request body)'\n    source: https://docs.api-swap-os.com/products/shipping/environments-and-auth/\n  - name: tlc-api-key\n    surface: TLC API\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    source: https://docs.api-swap-os.com/products/tlc/environments-and-auth/\nwebhook_verification:\n  - surface: Returns webhooks\n    method: JWT (HS256) in top-level jwt body field; secret whsk_<hex>; 5-minute expiry\n    source: https://docs.api-swap-os.com/products/returns/webhooks/\n\
  \  - surface: Shipping webhooks (orderCreated, labelUpdated)\n    method: HMAC-SHA256 Base64 signature in x-swap-signature-sha256 header; per-webhook signing secret\n    source: https://docs.api-swap-os.com/products/shipping/values-webhook/\n  - surface: Protect webhooks\n    method: JWT-signed payload\n    source: https://docs.api-swap-os.com/products/protect/protect-webhooks/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swap/refs/heads/main/authentication/swap-authentication.yml
summary_line: apiKey/http · 8 schemes
tags:
- Company
- E-Commerce
- Cross-Border
- Customs
- Shipping
- Returns
- Tax
- Duties
- Agentic Commerce
- Checkout
- Package Protection
- Landed Cost
---
