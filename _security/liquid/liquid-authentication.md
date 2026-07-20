---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Liquid Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- refresh_token
overview: Liquid secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code and refresh_token flow(s).
provider_name: Liquid
provider_slug: liquid
scheme_count: 1
schemes:
- applies_to: https://coinvest.liquid.trade/mcp
  challenge_observed: 'WWW-Authenticate: Bearer realm="mcp", resource_metadata="https://coinvest.liquid.trade/.well-known/oauth-protected-resource" (HTTP 401, verified 2026-07-19)'
  code_challenge_methods_supported:
  - S256
  endpoints:
    authorization: https://coinvest.liquid.trade/oauth/authorize
    introspection: https://coinvest.liquid.trade/oauth/introspect
    registration: https://coinvest.liquid.trade/oauth/register
    token: https://coinvest.liquid.trade/oauth/token
  flows:
  - authorizationUrl: https://coinvest.liquid.trade/oauth/authorize
    flow: authorizationCode
    scopes:
      read: Market data, portfolio and account state
      trade: Placing and managing orders, always behind an explicit human confirmation
    tokenUrl: https://coinvest.liquid.trade/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://coinvest.liquid.trade
  name: CoInvestOAuth
  response_types_supported:
  - code
  sources:
  - https://coinvest.liquid.trade/.well-known/oauth-authorization-server
  - https://coinvest.liquid.trade/.well-known/oauth-protected-resource
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
slug: liquid-authentication
source_filename: liquid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://coinvest.liquid.trade/.well-known/oauth-authorization-server\ndocs: https://www.liquid.trade/coinvest-docs\nnotes: >-\n  Liquid publishes no public REST API and no OpenAPI, so this profile is not derived from a spec. It is\n  transcribed from the live OAuth 2.0 Authorization Server Metadata (RFC 8414) and Protected Resource\n  Metadata (RFC 9728) documents served by the Co-Invest MCP host, plus the provider's Co-Invest\n  documentation. End users authenticate to the product itself with email sign-in or a crypto wallet;\n  machine/agent access is exclusively OAuth against the MCP server.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  dynamic_client_registration: true\n  bearer_methods:\n  - header\nschemes:\n- name: CoInvestOAuth\n  type: oauth2\n  applies_to: https://coinvest.liquid.trade/mcp\n  sources:\n  - https://coinvest.liquid.trade/.well-known/oauth-authorization-server\n\
  \  - https://coinvest.liquid.trade/.well-known/oauth-protected-resource\n  issuer: https://coinvest.liquid.trade\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coinvest.liquid.trade/oauth/authorize\n    tokenUrl: https://coinvest.liquid.trade/oauth/token\n    scopes:\n      read: Market data, portfolio and account state\n      trade: Placing and managing orders, always behind an explicit human confirmation\n  endpoints:\n    authorization: https://coinvest.liquid.trade/oauth/authorize\n    token: https://coinvest.liquid.trade/oauth/token\n    registration: https://coinvest.liquid.trade/oauth/register\n    introspection: https://coinvest.liquid.trade/oauth/introspect\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - none\n  challenge_observed: 'WWW-Authenticate: Bearer realm=\"mcp\", resource_metadata=\"\
  https://coinvest.liquid.trade/.well-known/oauth-protected-resource\"\n    (HTTP 401, verified 2026-07-19)'\nauthorization_boundaries:\n  granted:\n  - read market data, portfolio, positions, open orders and account state\n  - propose and, on explicit human confirmation, place and manage orders\n  never_granted:\n  - withdraw or transfer funds\n  - change account settings\n  - send an order without a Confirm tap\n  additional_gate: >-\n    First trade on a new account additionally requires the account to be funded and the trading agent\n    key to be approved in the browser; until then the server reports \"Trading not enabled\".\n  consent_warning: >-\n    Connections from MCP clients Liquid has not verified show an unverified-app warning on the sign-in\n    consent screen.\nend_user_authentication:\n  methods:\n  - email sign-in\n  - crypto wallet\n  source: https://docs.tryliquid.xyz/about-liquid/what-is-liquid\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid/refs/heads/main/authentication/liquid-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Crypto Defi
- Trading
- Perpetual Futures
- Prediction Markets
- Fintech
- MCP
- Agentic Commerce
- OAuth
---
