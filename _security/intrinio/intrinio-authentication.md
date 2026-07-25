---
api_key_in:
- query
- header
auth_types:
- apiKey
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Intrinio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Intrinio secures its APIs with apiKey, http-bearer, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Intrinio
provider_slug: intrinio
scheme_count: 4
schemes:
- description: Primary authentication for the Intrinio Web API v2 — include your API key as an api_key URL parameter, e.g. https://api-v2.intrinio.com/securities/AAPL/prices?api_key={api_key}.
  in: query
  name: api_key_query
  parameter: api_key
  sources:
  - https://docs.intrinio.com/documentation/api_v2/authentication
  type: apiKey
- description: Header alternative — send the API key as an Authorization header with the value "Bearer {api_key}".
  name: authorization_bearer
  scheme: bearer
  sources:
  - https://docs.intrinio.com/documentation/api_v2/authentication
  type: http
- description: Public-key authentication for untrusted/client-side environments (browser JavaScript). Public API keys are created on the account page and are domain-restricted — requests from unlisted domains are rejected with 401. localhost is whitelisted by default for development and should be removed before production.
  in: header
  name: public_api_key
  parameter: X-Authorization-Public-Key
  sources:
  - https://docs.intrinio.com/documentation/api_v2/authentication
  type: apiKey
- description: The hosted Intrinio MCP server (https://intrinio-mcp.intrinio.com/mcp) uses OAuth 2.0 authorization-code + refresh-token grants with PKCE (S256) and anonymous dynamic client registration; single scope "intrinio". API-key auth is also accepted per the MCP product page.
  flows:
  - authorizationUrl: https://intrinio-mcp.intrinio.com/authorize
    flow: authorizationCode
    scopes:
    - intrinio
    tokenUrl: https://intrinio-mcp.intrinio.com/token
  name: mcp_oauth
  sources:
  - https://intrinio-mcp.intrinio.com/.well-known/oauth-authorization-server
  - https://intrinio.com/mcp
  type: oauth2
slug: intrinio-authentication
source_filename: intrinio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\ndocs: https://docs.intrinio.com/documentation/api_v2/authentication\nsummary:\n  types: [apiKey, http-bearer, oauth2]\n  api_key_in: [query, header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: api_key_query\n    type: apiKey\n    in: query\n    parameter: api_key\n    description: >-\n      Primary authentication for the Intrinio Web API v2 — include your API key as an\n      api_key URL parameter, e.g.\n      https://api-v2.intrinio.com/securities/AAPL/prices?api_key={api_key}.\n    sources: [https://docs.intrinio.com/documentation/api_v2/authentication]\n  - name: authorization_bearer\n    type: http\n    scheme: bearer\n    description: >-\n      Header alternative — send the API key as an Authorization header with the value\n      \"Bearer {api_key}\".\n    sources: [https://docs.intrinio.com/documentation/api_v2/authentication]\n  - name: public_api_key\n    type: apiKey\n    in: header\n    parameter: X-Authorization-Public-Key\n\
  \    description: >-\n      Public-key authentication for untrusted/client-side environments (browser\n      JavaScript). Public API keys are created on the account page and are\n      domain-restricted — requests from unlisted domains are rejected with 401.\n      localhost is whitelisted by default for development and should be removed\n      before production.\n    sources: [https://docs.intrinio.com/documentation/api_v2/authentication]\n  - name: mcp_oauth\n    type: oauth2\n    description: >-\n      The hosted Intrinio MCP server (https://intrinio-mcp.intrinio.com/mcp) uses OAuth\n      2.0 authorization-code + refresh-token grants with PKCE (S256) and anonymous\n      dynamic client registration; single scope \"intrinio\". API-key auth is also\n      accepted per the MCP product page.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://intrinio-mcp.intrinio.com/authorize\n        tokenUrl: https://intrinio-mcp.intrinio.com/token\n        scopes: [intrinio]\n\
  \    sources:\n      - https://intrinio-mcp.intrinio.com/.well-known/oauth-authorization-server\n      - https://intrinio.com/mcp\nnotes: >-\n  Failed authentication returns HTTP 401 with a JSON body of the shape\n  {\"error\": \"API Key was invalid.\", \"message\": \"API Key was formatted invalidly.\"}\n  (observed live against api-v2.intrinio.com).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intrinio/refs/heads/main/authentication/intrinio-authentication.yml
summary_line: apiKey/http-bearer/oauth2 · 4 schemes
tags:
- Finance
- Financial Data
- Market Data
- Stocks
- Options
- Fundamentals
- ETFs
- Real-Time Data
---
