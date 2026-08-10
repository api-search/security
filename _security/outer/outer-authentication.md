---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Outer Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: Outer secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: Outer
provider_slug: outer
scheme_count: 1
schemes:
- authorizationUrl: https://account.liveouter.com/authentication/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  endSessionUrl: https://account.liveouter.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/11846615098
  jwksUri: https://account.liveouter.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccount
  openIdConnectUrl: https://liveouter.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/outer-openid-configuration.json
  - well-known/outer-oauth-authorization-server.json
  subject_types_supported:
  - public
  tokenUrl: https://account.liveouter.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: outer-authentication
source_filename: outer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://liveouter.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Derived from the live OIDC / RFC 8414 discovery documents served at liveouter.com, not from\n  an OpenAPI (Outer publishes none). The authorization server is Shopify's Customer Account\n  API issuer for shop id 11846615098, fronted on Outer's own account.liveouter.com host.\n  The UCP MCP endpoint at /api/ucp/mcp uses a different gate: it requires a resolvable UCP\n  agent profile URI rather than an OAuth token, and buyer payment approval on top.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\n  pkce: [S256]\nschemes:\n- name: ShopifyCustomerAccount\n  type: openIdConnect\n  openIdConnectUrl: https://liveouter.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/11846615098\n  authorizationUrl: https://account.liveouter.com/authentication/oauth/authorize\n\
  \  tokenUrl: https://account.liveouter.com/authentication/oauth/token\n  endSessionUrl: https://account.liveouter.com/authentication/logout\n  jwksUri: https://account.liveouter.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources:\n  - well-known/outer-openid-configuration.json\n  - well-known/outer-oauth-authorization-server.json\nagent_surface:\n  endpoint: https://liveouter.com/api/ucp/mcp\n  gate: UCP agent profile URI (HTTP 422 invalid_profile_url without one)\n  human_in_the_loop: required for complete_checkout (buyer must approve payment)\nx-evidence:\n\
  \  fetched: '2026-08-04'\n  urls:\n  - url: https://liveouter.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://liveouter.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://account.liveouter.com/authentication/.well-known/jwks.json\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outer/refs/heads/main/authentication/outer-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Retail
- E-Commerce
- Consumer Goods
- Furniture
- Home
- Direct to Consumer
- Agentic Commerce
- Shopify
- Universal Commerce Protocol
---
