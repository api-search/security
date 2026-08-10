---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- none
description: ''
kind: authentication
layout: security
method: searched
name: Super Coffee Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: Super Coffee secures its APIs with oauth2, openIdConnect, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: Super Coffee
provider_slug: super-coffee
scheme_count: 3
schemes:
- description: The UCP MCP endpoint answers tools/list and catalog/cart/checkout tool calls without credentials. Identity is asserted per call via the required meta.ucp-agent.profile URI rather than a bearer token. Payment completion is gated on an approved buyer payment instrument plus contemporaneous human approval, not on API authentication.
  evidence: anonymous POST tools/list returned HTTP 200 with 13 tools on 2026-08-05
  name: ucp-mcp-anonymous
  sources:
  - https://www.drinksupercoffee.com/api/ucp/mcp
  type: none
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  description: OpenID Connect for Shopify customer accounts on this storefront.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/14905858
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://www.drinksupercoffee.com/.well-known/openid-configuration
  sources:
  - https://www.drinksupercoffee.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
- description: OAuth 2.0 Authorization Server Metadata (RFC 8414) for customer accounts.
  end_session_endpoint: https://shopify.com/authentication/14905858/logout
  flows:
  - authorizationUrl: https://shopify.com/authentication/14905858/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    pkce: true
    tokenUrl: https://shopify.com/authentication/14905858/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  jwks_uri: https://shopify.com/authentication/14905858/.well-known/jwks.json
  name: shopify-customer-account-oauth2
  scopes: see scopes/super-coffee-scopes.yml
  sources:
  - https://www.drinksupercoffee.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
slug: super-coffee-authentication
source_filename: super-coffee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://www.drinksupercoffee.com/.well-known/openid-configuration\ndocs: https://www.drinksupercoffee.com/agents.md\nnote: >-\n  Super Coffee publishes no OpenAPI, so this profile is not derived from\n  securitySchemes. It is read from the storefront's live OAuth 2.0 / OpenID\n  Connect discovery documents and from the observed behaviour of the UCP MCP\n  endpoint. The authorization server is operated by Shopify on Super Coffee's\n  behalf (shop id 14905858), not by Super Coffee.\nsummary:\n  types: [oauth2, openIdConnect, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\n  anonymous_surface: true\nschemes:\n- name: ucp-mcp-anonymous\n  type: none\n  description: >-\n    The UCP MCP endpoint answers tools/list and catalog/cart/checkout tool calls\n    without credentials. Identity is asserted per call via the required meta.ucp-agent.profile\n    URI rather than a bearer token. Payment completion\
  \ is gated on an approved buyer\n    payment instrument plus contemporaneous human approval, not on API authentication.\n  sources:\n  - https://www.drinksupercoffee.com/api/ucp/mcp\n  evidence: anonymous POST tools/list returned HTTP 200 with 13 tools on 2026-08-05\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.drinksupercoffee.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/14905858\n  description: OpenID Connect for Shopify customer accounts on this storefront.\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources:\n  - https://www.drinksupercoffee.com/.well-known/openid-configuration\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  description: OAuth 2.0 Authorization Server Metadata (RFC 8414) for customer accounts.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://shopify.com/authentication/14905858/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/14905858/oauth/token\n    pkce: true\n    code_challenge_methods_supported: [S256]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  jwks_uri: https://shopify.com/authentication/14905858/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/14905858/logout\n  scopes: see scopes/super-coffee-scopes.yml\n  sources:\n  - https://www.drinksupercoffee.com/.well-known/oauth-authorization-server\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://www.drinksupercoffee.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://www.drinksupercoffee.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://www.drinksupercoffee.com/api/ucp/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-coffee/refs/heads/main/authentication/super-coffee-authentication.yml
summary_line: oauth2/openIdConnect/none · 3 schemes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
