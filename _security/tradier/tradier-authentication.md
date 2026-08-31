---
api_key_in: []
api_specs:
- filename: tradier-asyncapi.yml
  format: yaml
  label: Tradier Streaming API
  slug: streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/asyncapi/tradier-asyncapi.yml
- filename: tradier-accounts-api-openapi.yml
  format: yaml
  label: Tradier Accounts API
  slug: tradier-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-accounts-api-openapi.yml
- filename: tradier-market-data-api-openapi.yml
  format: yaml
  label: Tradier Market Data API
  slug: tradier-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-market-data-api-openapi.yml
- filename: tradier-options-api-openapi.yml
  format: yaml
  label: Tradier Options API
  slug: tradier-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-options-api-openapi.yml
- filename: tradier-streaming-api-openapi.yml
  format: yaml
  label: Tradier Streaming API
  slug: tradier-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-streaming-api-openapi.yml
- filename: tradier-trading-api-openapi.yml
  format: yaml
  label: Tradier Trading API
  slug: tradier-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-trading-api-openapi.yml
- filename: tradier-user-api-openapi.yml
  format: yaml
  label: Tradier User API
  slug: tradier-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-user-api-openapi.yml
- filename: tradier-watchlists-api-openapi.yml
  format: yaml
  label: Tradier Watchlists API
  slug: tradier-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-watchlists-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tradier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tradier secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tradier
provider_slug: tradier
scheme_count: 2
schemes:
- bearerFormat: OAuth2 access token
  description: 'Tradier OAuth 2.0 bearer token sent as `Authorization: Bearer <token>`. Individual developers use the personal API token (or Sandbox token) from https://dash.tradier.com/settings/api directly as the bearer token — no OAuth dance required.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tradier-openapi.yml
  type: http
- description: OAuth 2.0 authorization-code flow for approved Tradier partners building public applications. Authorization codes live 10 minutes; access tokens live 24 hours; refresh tokens never expire but are available to approved partners only (techsupport@tradier.com). Token exchange uses HTTP Basic auth with base64(clientID:clientSecret).
  flows:
  - authorizationUrl: https://api.tradier.com/v1/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.tradier.com/v1/oauth/refreshtoken
    scopes: 5
    tokenUrl: https://api.tradier.com/v1/oauth/accesstoken
  name: oauth2
  sources:
  - https://docs.tradier.com/docs/authentication
  type: oauth2
slug: tradier-authentication
source_filename: tradier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/tradier-openapi.yml\ndocs: https://docs.tradier.com/docs/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2 access token\n  description: 'Tradier OAuth 2.0 bearer token sent as `Authorization: Bearer <token>`. Individual developers use the personal API token (or Sandbox token) from https://dash.tradier.com/settings/api directly as the bearer token — no OAuth dance required.'\n  sources:\n  - openapi/tradier-openapi.yml\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code flow for approved Tradier partners building\n    public applications. Authorization codes live 10 minutes; access tokens live\n    24 hours; refresh tokens never expire but are available to approved partners\n    only (techsupport@tradier.com). Token exchange uses HTTP Basic auth with\n \
  \   base64(clientID:clientSecret).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.tradier.com/v1/oauth/authorize\n    tokenUrl: https://api.tradier.com/v1/oauth/accesstoken\n    refreshUrl: https://api.tradier.com/v1/oauth/refreshtoken\n    scopes: 5\n  sources:\n  - https://docs.tradier.com/docs/authentication\nscopes_artifact: scopes/tradier-scopes.yml\nmcp_auth:\n  note: >-\n    The hosted MCP server (mcp.tradier.com) authenticates with the same API token\n    via an API_KEY header or api_key query parameter plus a PAPER_TRADING flag,\n    and separately publishes RFC 8414 OAuth metadata (issuer\n    https://p-be-auth.tradier.com, scopes openid/mcp/claudeai, PKCE S256) — see\n    well-known/tradier-mcp-oauth-authorization-server.json.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/authentication/tradier-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fintech
- Trading
- Stocks
- Options
- Brokerage
- Streaming
---
