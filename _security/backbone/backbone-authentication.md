---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Backbone Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Backbone secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Backbone
provider_slug: backbone
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/36563550340/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/36563550340/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/36563550340
  jwks_uri: https://shopify.com/authentication/36563550340/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://backbone.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/backbone-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/36563550340/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: backbone-authentication
source_filename: backbone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://backbone.com/.well-known/openid-configuration\nnotes: >-\n  Auth metadata published on backbone.com is the Shopify Customer Account OIDC /\n  OAuth2 authorization server (issuer shopify.com/authentication/36563550340). It\n  governs customer-account login and the Shopify Customer Account API + Customer\n  Account MCP API. There is no first-party Backbone developer API; this is the\n  real, published auth surface for the store.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: [S256]\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://backbone.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/36563550340\n  authorization_endpoint: https://shopify.com/authentication/36563550340/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/36563550340/oauth/token\n  end_session_endpoint:\
  \ https://shopify.com/authentication/36563550340/logout\n  jwks_uri: https://shopify.com/authentication/36563550340/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  code_challenge_methods: [S256]\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources: [well-known/backbone-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backbone/refs/heads/main/authentication/backbone-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Entertainment
- Gaming
- Mobile Gaming
- Gaming Controller
- Consumer Electronics
- Hardware
- Ecommerce
---
