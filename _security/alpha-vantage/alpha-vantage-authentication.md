---
api_key_in:
- query
api_specs:
- filename: alpha-vantage-stock-time-series-api-openapi.yml
  format: yaml
  label: Alpha Vantage Stock Time Series API
  slug: alpha-vantage-stock-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/openapi/alpha-vantage-stock-time-series-api-openapi.yml
- filename: alpha-vantage-query-api-openapi.yml
  format: yaml
  label: Alpha Vantage Query API
  slug: alpha-vantage-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/openapi/alpha-vantage-query-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Alpha Vantage Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Alpha Vantage secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Alpha Vantage
provider_slug: alpha-vantage
scheme_count: 2
schemes:
- description: Alpha Vantage API key passed as apikey query parameter on every request to https://www.alphavantage.co/query. Free keys are claimed self-serve with an email address at https://www.alphavantage.co/support/#api-key and have lifetime access; premium keys raise rate limits. The literal key `demo` works for the documented example queries.
  in: query
  name: ApiKey
  parameter: apikey
  sources:
  - openapi/alpha-vantage-stock-time-series-api-openapi.yml
  - openapi/alpha-vantage-plugin-openapi.json
  type: apiKey
- description: 'The official MCP server (https://mcp.alphavantage.co/mcp) fronts the API key with OAuth 2.0 authorization-code + PKCE (S256) and dynamic client registration (RFC 8414 metadata published at /.well-known/oauth-authorization-server); the authorization page collects the user''s Alpha Vantage API key. Scope: alphavantage:read. Legacy API-key-in-URL connection (https://mcp.alphavantage.co/mcp?apikey=KEY) is documented as deprecated.'
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.alphavantage.co/authorize
      scopes:
        alphavantage:read: Read access to Alpha Vantage market data via MCP
      tokenUrl: https://mcp.alphavantage.co/token
  name: AlphaVantageMCPOAuth
  sources:
  - well-known/alpha-vantage-mcp-oauth-authorization-server.json
  - https://github.com/alphavantage/alpha_vantage_mcp
  type: oauth2
slug: alpha-vantage-authentication
source_filename: alpha-vantage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://www.alphavantage.co/support/#api-key\ndocs: https://www.alphavantage.co/documentation/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: >-\n    Alpha Vantage API key passed as apikey query parameter on every request to\n    https://www.alphavantage.co/query. Free keys are claimed self-serve with an email address at\n    https://www.alphavantage.co/support/#api-key and have lifetime access; premium keys raise rate\n    limits. The literal key `demo` works for the documented example queries.\n  sources:\n  - openapi/alpha-vantage-stock-time-series-api-openapi.yml\n  - openapi/alpha-vantage-plugin-openapi.json\n- name: AlphaVantageMCPOAuth\n  type: oauth2\n  description: >-\n    The official MCP server (https://mcp.alphavantage.co/mcp) fronts the API key with OAuth 2.0\n\
  \    authorization-code + PKCE (S256) and dynamic client registration (RFC 8414 metadata published at\n    /.well-known/oauth-authorization-server); the authorization page collects the user's Alpha Vantage\n    API key. Scope: alphavantage:read. Legacy API-key-in-URL connection\n    (https://mcp.alphavantage.co/mcp?apikey=KEY) is documented as deprecated.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.alphavantage.co/authorize\n      tokenUrl: https://mcp.alphavantage.co/token\n      scopes:\n        alphavantage:read: Read access to Alpha Vantage market data via MCP\n  sources:\n  - well-known/alpha-vantage-mcp-oauth-authorization-server.json\n  - https://github.com/alphavantage/alpha_vantage_mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/authentication/alpha-vantage-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Fintech
- Market Data
- Stocks
- FX
- Crypto
- Commodities
- Economic Indicators
- Technical Indicators
- Fundamentals
- News
- Sentiment
- Free
---
