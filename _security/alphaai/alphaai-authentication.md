---
api_key_in:
- header
api_specs:
- filename: alphaai-calendar-api-openapi.yml
  format: yaml
  label: AlphaAI Calendar API
  slug: alphaai-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/openapi/alphaai-calendar-api-openapi.yml
- filename: alphaai-news-api-openapi.yml
  format: yaml
  label: AlphaAI News API
  slug: alphaai-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/openapi/alphaai-news-api-openapi.yml
- filename: alphaai-symbols-api-openapi.yml
  format: yaml
  label: AlphaAI Symbols API
  slug: alphaai-symbols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/openapi/alphaai-symbols-api-openapi.yml
auth_types:
- http
- oauth2
description: Two authentication surfaces on two hosts. The REST API takes a single static bearer API key with a recognisable `ak_live_` prefix. The MCP server accepts either the SAME key as a bearer token or a full OAuth 2.1 authorization-code flow with PKCE and RFC 7591 dynamic client registration — the dual path is deliberate, so browserless agents (n8n, cron, CI) are not locked out of MCP.
kind: authentication
layout: security
method: searched
name: Alphaai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AlphaAI secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AlphaAI
provider_slug: alphaai
scheme_count: 3
schemes:
- applies_to: https://api.alphai.io
  bearerFormat: ak_live_*
  constraints:
  - Header only. The docs state explicitly that keys never go in a query parameter.
  - Send API traffic to api.alphai.io directly rather than through the website host — the provider notes the API host has no browser-oriented bot filtering.
  description: 'Token of the form `ak_live_<random>`. Issued from

    `/account/api-keys` on the website. Send as `Authorization: Bearer …`.'
  header: Authorization
  in: header
  key_management:
    credit_card_required: false
    issue_url: https://alphai.io/account/api-keys
    keys_per_account:
      Basic: 1
      Free: 1
      Pro: 5
    rotation: Keys can be revoked from the dashboard; a revoked key returns 401 "Invalid or revoked API key."
  name: apiKey
  required_on: every request (global security requirement in the spec)
  scheme: bearer
  sources:
  - openapi/alphaai-rest-api-openapi.yml
  type: http
- applies_to: https://mcp.alphai.io/mcp
  detail: scopes/alphaai-scopes.yml
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.alphai.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://mcp.alphai.io/oauth/token
    scopes:
    - tools.read
    - tools.bulk
    tokenUrl: https://mcp.alphai.io/oauth/token
  name: MCP OAuth 2.1
  registration_endpoint: https://mcp.alphai.io/oauth/register
  sources:
  - well-known/alphaai-oauth-authorization-server.json
  - well-known/alphaai-oauth-protected-resource.json
  type: oauth2
- applies_to: https://mcp.alphai.io/mcp
  bearerFormat: ak_live_*
  description: The REST key used as an MCP bearer token, for clients with no browser to run the OAuth flow. Documented at https://alphai.io/mcp.
  name: MCP bearer (API key)
  scheme: bearer
  sources:
  - https://alphai.io/mcp
  type: http
slug: alphaai-authentication
source_filename: alphaai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: openapi/alphaai-rest-api-openapi.yml\ndocs: https://alphai.io/developers\ndescription: >-\n  Two authentication surfaces on two hosts. The REST API takes a single static\n  bearer API key with a recognisable `ak_live_` prefix. The MCP server accepts\n  either the SAME key as a bearer token or a full OAuth 2.1 authorization-code\n  flow with PKCE and RFC 7591 dynamic client registration — the dual path is\n  deliberate, so browserless agents (n8n, cron, CI) are not locked out of MCP.\n\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n\nschemes:\n  - name: apiKey\n    type: http\n    scheme: bearer\n    bearerFormat: ak_live_*\n    in: header\n    header: Authorization\n    applies_to: https://api.alphai.io\n    description: |-\n      Token of the form `ak_live_<random>`. Issued from\n      `/account/api-keys` on the website. Send as `Authorization: Bearer …`.\n    sources:\n  \
  \    - openapi/alphaai-rest-api-openapi.yml\n    required_on: every request (global security requirement in the spec)\n    key_management:\n      issue_url: https://alphai.io/account/api-keys\n      credit_card_required: false\n      keys_per_account: {Free: 1, Basic: 1, Pro: 5}\n      rotation: Keys can be revoked from the dashboard; a revoked key returns 401 \"Invalid or revoked API key.\"\n    constraints:\n      - Header only. The docs state explicitly that keys never go in a query parameter.\n      - >-\n        Send API traffic to api.alphai.io directly rather than through the\n        website host — the provider notes the API host has no browser-oriented\n        bot filtering.\n\n  - name: MCP OAuth 2.1\n    type: oauth2\n    applies_to: https://mcp.alphai.io/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.alphai.io/oauth/authorize\n        tokenUrl: https://mcp.alphai.io/oauth/token\n        refreshUrl: https://mcp.alphai.io/oauth/token\n\
  \        scopes: [tools.read, tools.bulk]\n        pkce: S256\n    dynamic_client_registration: true\n    registration_endpoint: https://mcp.alphai.io/oauth/register\n    sources:\n      - well-known/alphaai-oauth-authorization-server.json\n      - well-known/alphaai-oauth-protected-resource.json\n    detail: scopes/alphaai-scopes.yml\n\n  - name: MCP bearer (API key)\n    type: http\n    scheme: bearer\n    bearerFormat: ak_live_*\n    applies_to: https://mcp.alphai.io/mcp\n    description: >-\n      The REST key used as an MCP bearer token, for clients with no browser to\n      run the OAuth flow. Documented at https://alphai.io/mcp.\n    sources: [https://alphai.io/mcp]\n\nfailure_modes:\n  - status: 401\n    when: no Authorization header\n    body: '{\"detail\": \"API key required.\"}'\n    observed: '2026-08-11'\n  - status: 401\n    when: malformed / revoked key\n    body: '{\"message\":\"Invalid or revoked API key.\",\"extra\":{}}'\n    headers: 'WWW-Authenticate: Bearer'\n    observed:\
  \ '2026-08-11'\n  - status: 401\n    when: MCP request with no token\n    body_fields: [error, reason, how_to_connect]\n    headers: 'WWW-Authenticate: Bearer realm=\"alphai-mcp\", resource_metadata=\"https://mcp.alphai.io/.well-known/oauth-protected-resource/mcp\"'\n    observed: '2026-08-11'\n    note: >-\n      A model 401 — it names the resource metadata document AND carries a plain\n      how_to_connect string telling the caller where to create a key.\n\nnotes:\n  - >-\n    The two 401 envelopes on the REST API are inconsistent: a missing key returns\n    a `detail` field, an invalid key returns `message` + `extra`. Both shapes are\n    permitted by the spec's Error schema, but an agent has to handle both.\n  - >-\n    There is no per-key scoping on REST. A key is a whole-account credential; the\n    only differentiation is plan tier.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/authentication/alphaai-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Financial News
- Stock Market
- SEC Filings
- Insider Trading
- Fintech
- Market Data
- Sentiment
- AI Agents
- MCP
- LLM
- Trading
---
