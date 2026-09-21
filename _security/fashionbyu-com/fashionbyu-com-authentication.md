---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: fashionbyu-com-iriz-platform-api-openapi.yml
  format: yaml
  label: IRIZ Platform API
  slug: iriz-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fashionbyu-com/refs/heads/main/openapi/fashionbyu-com-iriz-platform-api-openapi.yml
auth_types:
- apiKey
- http
- none
- hmac-signature
- http-message-signature
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Fashionbyu Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: IRIZ Platform secures its APIs with apiKey, http, none, hmac-signature, and http-message-signature across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IRIZ Platform
provider_slug: fashionbyu-com
scheme_count: 6
schemes:
- description: Platform gateway password or token
  in: query
  name: apiKey
  parameter: p
  sources:
  - openapi/fashionbyu-com-iriz-platform-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fashionbyu-com-iriz-platform-api-openapi.yml
  type: http
- applies_to:
  - MCP create_cart, mutate_cart, quote_cart, confirm_checkout
  - POST /iriz/v1/agent/cart/session (401 "Agent token required when configured")
  conditional: true
  description: '"Authorization: Bearer <IRIZ_AGENT_COMMERCE_TOKEN> when configured" — the commerce agent card records token_required: false and the read tools were called live without a token'
  name: agent-commerce-bearer
  scheme: bearer
  sources:
  - mcp/fashionbyu-com-mcp-initialize.json
  - a2a/fashionbyu-com-agent-card.json
  type: http
- applies_to:
  - 'A2A interop: POST /iriz/interop/tasks (401 peer_credentials_required without it)'
  description: HMAC-SHA256(peer_secret, "<peer>.<ts>.<nonce>.<sha256(body)>") sent with x-iriz-peer-id, x-iriz-peer-ts, x-iriz-peer-nonce headers
  in: header
  name: peerHmac
  parameter: x-iriz-peer-sig
  sources:
  - a2a/fashionbyu-com-interop-agent-card.json
  type: apiKey
- applies_to:
  - A2A interop
  description: Short-lived token from POST /iriz/interop/token { peer_id, secret } (GET on that path is 404 endpoint_not_found; POST not attempted — requires a registered peer secret)
  name: interop-bearer
  scheme: bearer
  sources:
  - a2a/fashionbyu-com-interop-agent-card.json
  type: http
- applies_to:
  - A2A interop
  description: RFC 9421 HTTP message signature; verified signatures raise trust tier (declared, not verifiable anonymously)
  name: webBotAuth
  scheme: signature
  sources:
  - a2a/fashionbyu-com-interop-agent-card.json
  type: http
slug: fashionbyu-com-authentication
source_filename: fashionbyu-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/fashionbyu-com-iriz-platform-api-openapi.yml (securitySchemes) upgraded with the live 401 bodies observed\n  on 2026-09-19, the MCP server instructions (initialize) and GET /iriz/v1/agent/mcp write_auth, and the securitySchemes\n  of both A2A agent cards\nsummary:\n  types:\n  - apiKey\n  - http\n  - none\n  - hmac-signature\n  - http-message-signature\n  api_key_in:\n  - query\n  public_surface: Agent-commerce read routes and MCP tools/list, initialize and read tools answer with no credentials\n  auth_levels:\n    standard: GET /iriz/status, /iriz/version, /iriz/interop/status, /iriz/interop/a2ui/catalog -> 401 {\"code\":\"UNAUTHORIZED\",\"auth_level\":\"standard\"}\n    boss: GET /iriz/agent-commerce/status -> 401 auth_level boss; robots.txt disallows /boss/\n    issuance: not documented publicly on any readable page\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: p\n  description: Platform gateway\
  \ password or token\n  sources:\n  - openapi/fashionbyu-com-iriz-platform-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fashionbyu-com-iriz-platform-api-openapi.yml\n- name: agent-commerce-bearer\n  type: http\n  scheme: bearer\n  applies_to:\n  - MCP create_cart, mutate_cart, quote_cart, confirm_checkout\n  - POST /iriz/v1/agent/cart/session (401 \"Agent token required when configured\")\n  conditional: true\n  description: '\"Authorization: Bearer <IRIZ_AGENT_COMMERCE_TOKEN> when configured\" — the commerce agent card records token_required:\n    false and the read tools were called live without a token'\n  sources:\n  - mcp/fashionbyu-com-mcp-initialize.json\n  - a2a/fashionbyu-com-agent-card.json\n- name: peerHmac\n  type: apiKey\n  in: header\n  parameter: x-iriz-peer-sig\n  applies_to:\n  - 'A2A interop: POST /iriz/interop/tasks (401 peer_credentials_required without it)'\n  description: HMAC-SHA256(peer_secret,\
  \ \"<peer>.<ts>.<nonce>.<sha256(body)>\") sent with x-iriz-peer-id, x-iriz-peer-ts,\n    x-iriz-peer-nonce headers\n  sources:\n  - a2a/fashionbyu-com-interop-agent-card.json\n- name: interop-bearer\n  type: http\n  scheme: bearer\n  applies_to:\n  - A2A interop\n  description: Short-lived token from POST /iriz/interop/token { peer_id, secret } (GET on that path is 404 endpoint_not_found;\n    POST not attempted — requires a registered peer secret)\n  sources:\n  - a2a/fashionbyu-com-interop-agent-card.json\n- name: webBotAuth\n  type: http\n  scheme: signature\n  applies_to:\n  - A2A interop\n  description: RFC 9421 HTTP message signature; verified signatures raise trust tier (declared, not verifiable anonymously)\n  sources:\n  - a2a/fashionbyu-com-interop-agent-card.json\ndocs: https://mirror.fashionbyu.com/iriz/docs\noauth:\n  present: false\n  evidence: no oauth2/openIdConnect scheme in the spec; /.well-known/oauth-authorization-server, oauth-protected-resource\n    and openid-configuration\
  \ are 403 on fashionbyu.com and on the MCP host mirror.fashionbyu.com\nnote: The OpenAPI declares two schemes but applies neither to any operation (security is absent on 107 of 108 operations),\n  so the spec cannot say which routes need which credential; the applicability above is what the live server answered.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fashionbyu-com/refs/heads/main/authentication/fashionbyu-com-authentication.yml
summary_line: apiKey/http/none/hmac-signature/http-message-signature · 6 schemes
tags:
- Company
- Fashion
- E-Commerce
- Agentic Commerce
- Storefront
- Product Feeds
- MCP
- A2A
- AI Agents
- Checkout
- Cart
- Order
- Cloudflare Workers
---
