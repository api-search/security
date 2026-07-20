---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: 52Toys Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: 52TOYS secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: 52TOYS
provider_slug: 52toys
scheme_count: 1
schemes:
- authorization_endpoint: https://account.hi52toys.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.hi52toys.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/77378748731
  jwks_uri: https://account.hi52toys.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://hi52toys.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/52toys-openid-configuration.json
  token_endpoint: https://account.hi52toys.com/authentication/oauth/token
  type: openIdConnect
slug: 52toys-authentication
source_filename: 52toys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://hi52toys.com/.well-known/openid-configuration\ndocs: https://hi52toys.com/.well-known/oauth-authorization-server\nnote: >-\n  52TOYS has no traditional developer REST API; authentication here is the\n  Shopify customer-account identity surface backing agent-driven commerce (UCP\n  MCP) and shopper login on the hi52toys.com storefront. Discovered live via the\n  store's OpenID Connect and RFC 8414 metadata documents (identical payloads).\n  Read-only catalog browsing needs no auth.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\n  pkce: S256\n  token_endpoint_auth_methods: [client_secret_basic]\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/77378748731\n  openIdConnectUrl: https://hi52toys.com/.well-known/openid-configuration\n  authorization_endpoint: https://account.hi52toys.com/authentication/oauth/authorize\n\
  \  token_endpoint: https://account.hi52toys.com/authentication/oauth/token\n  end_session_endpoint: https://account.hi52toys.com/authentication/logout\n  jwks_uri: https://account.hi52toys.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  id_token_signing_alg: RS256\n  code_challenge_methods: [S256]\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources: [well-known/52toys-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/52toys/refs/heads/main/authentication/52toys-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Collectibles
- Toys
- Retail
- Ecommerce
- Shopify
- Agentic Commerce
---
