---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hill House Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hill House secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hill House
provider_slug: hill-house
scheme_count: 1
schemes:
- authorization_endpoint: https://account.hillhousehome.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.hillhousehome.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/9321794
  jwks_uri: https://account.hillhousehome.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://hillhousehome.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types_supported:
  - public
  token_endpoint: https://account.hillhousehome.com/authentication/oauth/token
  type: openIdConnect
slug: hill-house-authentication
source_filename: hill-house-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://hillhousehome.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nplatform: Shopify Customer Account API (OAuth 2.0 / OpenID Connect)\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://hillhousehome.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/9321794\n  authorization_endpoint: https://account.hillhousehome.com/authentication/oauth/authorize\n  token_endpoint: https://account.hillhousehome.com/authentication/oauth/token\n  end_session_endpoint: https://account.hillhousehome.com/authentication/logout\n  jwks_uri: https://account.hillhousehome.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n\
  \  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\nnotes:\n- The Storefront MCP server at https://hillhousehome.com/api/mcp is currently unauthenticated (public catalog/cart/policy tools).\n- Customer-scoped access (orders, account, customer-account MCP) uses the Shopify Customer Account OAuth flow above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hill-house/refs/heads/main/authentication/hill-house-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- E-commerce
- Retail
- Home Goods
- Apparel
- Direct to Consumer
- Consumer Brand
- Shopify
- MCP
---
