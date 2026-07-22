---
api_key_in:
- header
- query
api_specs:
- filename: top-group-tonapi-openapi.yml
  format: yaml
  label: TON API
  slug: tonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/top-group/refs/heads/main/openapi/top-group-tonapi-openapi.yml
- filename: top-group-tonapi-webhooks-openapi.yml
  format: yaml
  label: TON API Webhooks API
  slug: tonapi-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/top-group/refs/heads/main/openapi/top-group-tonapi-webhooks-openapi.yml
auth_types:
- http-bearer
- apiKey
description: Authentication profile for TON API (tonapi.io) and the TON API Webhooks API (rt.tonapi.io). The published OpenAPI declares no securitySchemes; this profile is captured from the official TON API documentation. REST API methods work unauthenticated at a heavily throttled rate; production use requires a bearer API token issued by TON Console. The Webhooks API always requires a private API key.
kind: authentication
layout: security
method: searched
name: Top Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: TOP Group (The Open Platform) secures its APIs with http-bearer and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TOP Group (The Open Platform)
provider_slug: top-group
scheme_count: 3
schemes:
- applies_to: https://tonapi.io, https://testnet.tonapi.io
  description: Obtain a token from https://tonconsole.com/ and pass it in the Authorization header using the Bearer scheme. All REST methods are also available without authentication at a rate limit of 1 request per 4 seconds (0.24 rps); authenticated rate limits match the purchased TON Console plan and apply equally to mainnet and testnet.
  docs: https://docs.tonconsole.com/tonapi
  name: TON Console API token (REST API)
  scheme: bearer
  type: http
- applies_to: https://rt.tonapi.io, https://rt-testnet.tonapi.io
  description: All Webhooks API methods require a private API key from TON Console. The key is read from the Authorization header (Bearer scheme) first, then from the "token" query-string parameter.
  docs: https://docs.tonconsole.com/tonapi/webhooks-api
  in: header-or-query
  name: Webhooks API private key
  type: apiKey
- description: The deprecated SSE/WebSocket Streaming API accepts requests without a key (limited concurrent connections) or a TON Console token via Authorization Bearer header or "token" query parameter.
  docs: https://docs.tonconsole.com/tonapi/streaming-api
  in: header-or-query
  name: Streaming API token (deprecated surface)
  type: apiKey
slug: top-group-authentication
source_filename: top-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tonconsole.com/tonapi\ndocs: https://docs.tonconsole.com/tonapi\ndescription: >-\n  Authentication profile for TON API (tonapi.io) and the TON API Webhooks API\n  (rt.tonapi.io). The published OpenAPI declares no securitySchemes; this\n  profile is captured from the official TON API documentation. REST API methods\n  work unauthenticated at a heavily throttled rate; production use requires a\n  bearer API token issued by TON Console. The Webhooks API always requires a\n  private API key.\nsummary:\n  types: [http-bearer, apiKey]\n  api_key_in: [header, query]\nschemes:\n- name: TON Console API token (REST API)\n  type: http\n  scheme: bearer\n  description: >-\n    Obtain a token from https://tonconsole.com/ and pass it in the\n    Authorization header using the Bearer scheme. All REST methods are also\n    available without authentication at a rate limit of 1 request per 4\n    seconds (0.24 rps); authenticated\
  \ rate limits match the purchased TON\n    Console plan and apply equally to mainnet and testnet.\n  docs: https://docs.tonconsole.com/tonapi\n  applies_to: https://tonapi.io, https://testnet.tonapi.io\n- name: Webhooks API private key\n  type: apiKey\n  in: header-or-query\n  description: >-\n    All Webhooks API methods require a private API key from TON Console. The\n    key is read from the Authorization header (Bearer scheme) first, then from\n    the \"token\" query-string parameter.\n  docs: https://docs.tonconsole.com/tonapi/webhooks-api\n  applies_to: https://rt.tonapi.io, https://rt-testnet.tonapi.io\n- name: Streaming API token (deprecated surface)\n  type: apiKey\n  in: header-or-query\n  description: >-\n    The deprecated SSE/WebSocket Streaming API accepts requests without a key\n    (limited concurrent connections) or a TON Console token via Authorization\n    Bearer header or \"token\" query parameter.\n  docs: https://docs.tonconsole.com/tonapi/streaming-api\nnotes:\n\
  - The published OpenAPI (openapi/top-group-tonapi-openapi.yml) declares no\n  components.securitySchemes; the auth model above is documented prose.\n- No OAuth2/OIDC surface is published, so no scopes/ artifact exists for this\n  provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/top-group/refs/heads/main/authentication/top-group-authentication.yml
summary_line: http-bearer/apiKey · 3 schemes
tags:
- Company
- Blockchain
- TON
- Telegram
- Crypto
- Wallets
- Web3
- NFT
- Payments
---
