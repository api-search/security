---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Fly By Jing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fly By Jing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fly By Jing
provider_slug: fly-by-jing
scheme_count: 1
schemes:
- authorization_endpoint: https://account.flybyjing.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.flybyjing.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/6585155653
  jwks_uri: https://account.flybyjing.com/authentication/.well-known/jwks.json
  name: shopify_customer_account_oidc
  openIdConnectUrl: https://flybyjing.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types_supported:
  - public
  token_endpoint: https://account.flybyjing.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: fly-by-jing-authentication
source_filename: fly-by-jing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  Live OIDC/OAuth discovery document fetched from\n  https://flybyjing.com/.well-known/openid-configuration (Shopify Customer\n  Account API bound to the Fly By Jing store domain).\nsummary: >-\n  Fly By Jing's storefront (Shopify) exposes a Customer Account API secured with\n  OAuth 2.0 / OpenID Connect. Authorization Code grant with PKCE (S256) is the\n  primary flow; refresh_token and the JWT-bearer grant are also supported.\nschemes:\n- name: shopify_customer_account_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://flybyjing.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/6585155653\n  authorization_endpoint: https://account.flybyjing.com/authentication/oauth/authorize\n  token_endpoint: https://account.flybyjing.com/authentication/oauth/token\n  end_session_endpoint: https://account.flybyjing.com/authentication/logout\n  jwks_uri: https://account.flybyjing.com/authentication/.well-known/jwks.json\n\
  \  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  scopes_supported:\n  - openid\n  - email\n  - 'customer-account-api:full'\n  - 'customer-account-mcp-api:full'\nnotes: >-\n  Endpoints and issuer are Shopify-operated; the store's own subdomain\n  (account.flybyjing.com) fronts the authorize/token/logout endpoints. See\n  scopes/fly-by-jing-scopes.yml for the scope reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fly-by-jing/refs/heads/main/authentication/fly-by-jing-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Shopify
- Direct to Consumer
- MCP
- Agentic Commerce
---
