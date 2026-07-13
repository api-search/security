---
api_key_in:
- header
api_specs:
- filename: kraken-spot-rest-openapi.yml
  format: yaml
  label: Kraken Spot REST API
  slug: kraken-spot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/openapi/kraken-spot-rest-openapi.yml
- filename: kraken-asyncapi.yml
  format: yaml
  label: Kraken Spot WebSocket API v2
  slug: kraken-spot-websocket-api-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/asyncapi/kraken-asyncapi.yml
- filename: kraken-futures-rest-openapi.yml
  format: yaml
  label: Kraken Futures REST API
  slug: kraken-futures-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/openapi/kraken-futures-rest-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kraken Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kraken secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kraken
provider_slug: kraken
scheme_count: 2
schemes:
- description: 'Kraken Futures signs requests with two headers: `APIKey` (public key) and `Authent` (base64 HMAC-SHA512 over `postData + nonce + endpointPath` using the SHA-256 hash of those values, then HMAC-SHA512 keyed by the base64-decoded secret). A `Nonce` header carries the incrementing nonce.'
  in: header
  name: futures_signature
  parameter: APIKey
  sources:
  - openapi/kraken-futures-rest-openapi.yml
  type: apiKey
- description: 'Kraken signs private REST requests with two headers: `API-Key` (your public API key) and `API-Sign` (HMAC-SHA512 of the URI path plus SHA256(nonce + POST body), keyed by the base64-decoded secret). All private endpoints must include an incrementing `nonce` in the POST body.'
  in: header
  name: kraken_signature
  parameter: API-Key
  sources:
  - openapi/kraken-spot-rest-openapi.yml
  type: apiKey
slug: kraken-authentication
source_filename: kraken-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kraken-futures-rest-openapi.yml, openapi/kraken-spot-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: futures_signature\n  type: apiKey\n  in: header\n  parameter: APIKey\n  description: 'Kraken Futures signs requests with two headers: `APIKey` (public key) and `Authent`\n    (base64 HMAC-SHA512 over `postData + nonce + endpointPath` using the SHA-256 hash of those\n    values, then HMAC-SHA512 keyed by the base64-decoded secret). A `Nonce` header carries the\n    incrementing nonce.'\n  sources:\n  - openapi/kraken-futures-rest-openapi.yml\n- name: kraken_signature\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: 'Kraken signs private REST requests with two headers: `API-Key` (your public\n    API key) and `API-Sign` (HMAC-SHA512 of the URI path plus SHA256(nonce + POST body), keyed\n    by the base64-decoded secret). All private endpoints must include\
  \ an incrementing `nonce`\n    in the POST body.'\n  sources:\n  - openapi/kraken-spot-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/authentication/kraken-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Spot Trading
- Futures
- Derivatives
- Staking
- Earn
- NFT
- WebSocket
- FIX
- Custody
- OTC
- Prime Brokerage
- Embed
- OAuth
- Public APIs
---
