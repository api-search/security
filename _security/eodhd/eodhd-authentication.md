---
api_key_in:
- query
api_specs:
- filename: eodhd-financial-data-openapi.yml
  format: yaml
  label: EODHD Financial Data API
  slug: financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/openapi/eodhd-financial-data-openapi.yml
- filename: eodhd-websockets-asyncapi.yml
  format: yaml
  label: EODHD WebSockets Real-Time API
  slug: websockets-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/asyncapi/eodhd-websockets-asyncapi.yml
- filename: eodhd-eod-api-openapi.yml
  format: yaml
  label: EODHD Eod API
  slug: eodhd-eod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/openapi/eodhd-eod-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Eodhd Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: EODHD secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: EODHD
provider_slug: eodhd
scheme_count: 2
schemes:
- in: query
  name: EODHDQueryKey
  notes: All REST endpoints authenticate with ?api_token=YOUR_API_KEY. No Authorization headers, no OAuth on the REST API. A public demo token (api_token=demo) is limited to AAPL.US, MSFT.US, TSLA.US, VTI.US, AMZN.US, SWPPX.US, EURUSD.FOREX, and BTC-USD.CC. The WebSocket API validates the same api_token during handshake. A non-TLS alternative host (http://nonsecure.eodhd.com/api) is published for MATLAB/R clients.
  parameter: api_token
  sources:
  - openapi/eodhd-financial-data-openapi.yml
  - openapi/eodhd-eod-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://mcpv2.eodhd.dev/authorize
    flow: authorizationCode
    pkce: S256
    scopes: 12 published scopes — see scopes/eodhd-scopes.yml
    tokenUrl: https://mcpv2.eodhd.dev/token
  name: EODHD MCP OAuth (v2)
  notes: Applies to the hosted MCP server v2 endpoint (https://mcpv2.eodhd.dev/v2/mcp, Bearer tokens only). Supports dynamic client registration (RFC 7591), token introspection, refresh tokens, and resource indicators (RFC 8707). MCP v1 accepts the REST API key as ?apikey= instead.
  sources:
  - well-known/eodhd-mcp-oauth-authorization-server.json
  type: oauth2
slug: eodhd-authentication
source_filename: eodhd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/eodhd-financial-data-openapi.yml + https://eodhd.com/llms.txt + https://mcpv2.eodhd.dev/.well-known/oauth-authorization-server\ndocs: https://eodhd.com/financial-apis/\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: EODHDQueryKey\n    type: apiKey\n    in: query\n    parameter: api_token\n    sources:\n      - openapi/eodhd-financial-data-openapi.yml\n      - openapi/eodhd-eod-api-openapi.yml\n    notes: >-\n      All REST endpoints authenticate with ?api_token=YOUR_API_KEY. No Authorization\n      headers, no OAuth on the REST API. A public demo token (api_token=demo) is\n      limited to AAPL.US, MSFT.US, TSLA.US, VTI.US, AMZN.US, SWPPX.US, EURUSD.FOREX,\n      and BTC-USD.CC. The WebSocket API validates the same api_token during handshake.\n      A non-TLS alternative host (http://nonsecure.eodhd.com/api) is published for\n      MATLAB/R clients.\n\
  \  - name: EODHD MCP OAuth (v2)\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcpv2.eodhd.dev/authorize\n        tokenUrl: https://mcpv2.eodhd.dev/token\n        pkce: S256\n        scopes: 12 published scopes — see scopes/eodhd-scopes.yml\n    sources:\n      - well-known/eodhd-mcp-oauth-authorization-server.json\n    notes: >-\n      Applies to the hosted MCP server v2 endpoint (https://mcpv2.eodhd.dev/v2/mcp,\n      Bearer tokens only). Supports dynamic client registration (RFC 7591), token\n      introspection, refresh tokens, and resource indicators (RFC 8707). MCP v1\n      accepts the REST API key as ?apikey= instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/authentication/eodhd-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Financial
- Market Data
- Stock Options
- Stocks
- ETFs
- Forex
- Cryptocurrency
- Fundamentals
- News
---
