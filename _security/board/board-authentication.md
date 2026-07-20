---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Board Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: Board secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: Board
provider_slug: board
scheme_count: 1
schemes:
- authorization_endpoint: https://account.board.fun/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.board.fun/authentication/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/93388013858
  jwks_uri: https://account.board.fun/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://board.fun/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://account.board.fun/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: board-authentication
source_filename: board-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://board.fun/.well-known/openid-configuration\nnotes: >-\n  Board authenticates buyers via Shopify Customer Accounts (OpenID Connect).\n  The OIDC discovery document is live at /.well-known/openid-configuration and\n  an RFC 8414 authorization-server metadata document at\n  /.well-known/oauth-authorization-server. Read-only catalog browsing needs no\n  authentication; transactional agent-commerce flows use OIDC + Shopify Shop Pay.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/93388013858\n  openIdConnectUrl: https://board.fun/.well-known/openid-configuration\n  authorization_endpoint: https://account.board.fun/authentication/oauth/authorize\n  token_endpoint: https://account.board.fun/authentication/oauth/token\n\
  \  end_session_endpoint: https://account.board.fun/authentication/logout\n  jwks_uri: https://account.board.fun/authentication/.well-known/jwks.json\n  response_types_supported:\n  - code\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/board/refs/heads/main/authentication/board-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Commerce
- E-Commerce
- Board Games
- Agent Commerce
- Universal Commerce Protocol
- Shopify
- MCP
---
