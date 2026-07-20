---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: 99 Counties Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 99 Counties secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 99 Counties
provider_slug: 99-counties
scheme_count: 1
schemes:
- authorization_endpoint: https://account.wallacefarms.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.wallacefarms.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/35071754378
  jwks_uri: https://account.wallacefarms.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/99-counties-openid-configuration.json
  token_endpoint: https://account.wallacefarms.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: 99-counties-authentication
source_filename: 99-counties-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://99counties.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  platform: Shopify Customer Account (OIDC)\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/35071754378\n  authorization_endpoint: https://account.wallacefarms.com/authentication/oauth/authorize\n  token_endpoint: https://account.wallacefarms.com/authentication/oauth/token\n  end_session_endpoint: https://account.wallacefarms.com/authentication/logout\n  jwks_uri: https://account.wallacefarms.com/authentication/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n\
  \  - RS256\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/99-counties-openid-configuration.json\nnotes: >-\n  Storefront browsing and UCP catalog reads are unauthenticated. Authenticated\n  customer-account access (orders, membership, and the customer-account MCP API)\n  uses Shopify Customer Account OAuth 2.0 / OIDC with PKCE (S256). Agent checkout\n  is gated on buyer approval rather than an agent-held credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99-counties/refs/heads/main/authentication/99-counties-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- E-Commerce
- Agent Commerce
- Regenerative Agriculture
- Food and Beverage
- Shopify
- Model Context Protocol
- Universal Commerce Protocol
---
