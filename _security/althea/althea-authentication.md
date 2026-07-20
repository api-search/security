---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Althea Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Althea secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Althea
provider_slug: althea
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/9377939535/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/9377939535/logout
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/9377939535
  jwks_uri: https://shopify.com/authentication/9377939535/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://us.althea.kr/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/althea-openid-configuration.json
  - well-known/althea-oauth-authorization-server.json
  token_endpoint: https://shopify.com/authentication/9377939535/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: althea-authentication
source_filename: althea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://us.althea.kr/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Customer-facing auth is Shopify Customer Accounts (OpenID Connect). Agent\n    read/transact access to the storefront MCP is unauthenticated for browsing;\n    checkout requires buyer approval via Shop Pay / UCP.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://us.althea.kr/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/9377939535\n  authorization_endpoint: https://shopify.com/authentication/9377939535/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/9377939535/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/9377939535/logout\n  jwks_uri: https://shopify.com/authentication/9377939535/.well-known/jwks.json\n  response_types: [code]\n  id_token_signing_alg:\
  \ [RS256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  scopes: [openid, email, customer-account-api:full, customer-account-mcp-api:full]\n  sources: [well-known/althea-openid-configuration.json, well-known/althea-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/althea/refs/heads/main/authentication/althea-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- E-Commerce
- Retail
- Beauty
- Cosmetics
- K-Beauty
- Skincare
- Agent Commerce
- Shopify
---
