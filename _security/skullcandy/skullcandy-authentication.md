---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Skullcandy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Skullcandy secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Skullcandy
provider_slug: skullcandy
scheme_count: 1
schemes:
- authorization_endpoint: https://account.skullcandy.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.skullcandy.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/63551143993
  jwks_uri: https://account.skullcandy.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://skullcandy.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/skullcandy-openid-configuration.json
  token_endpoint: https://account.skullcandy.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: skullcandy-authentication
source_filename: skullcandy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://skullcandy.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  issuer: https://shopify.com/authentication/63551143993\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://skullcandy.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/63551143993\n  authorization_endpoint: https://account.skullcandy.com/authentication/oauth/authorize\n  token_endpoint: https://account.skullcandy.com/authentication/oauth/token\n  end_session_endpoint: https://account.skullcandy.com/authentication/logout\n  jwks_uri: https://account.skullcandy.com/authentication/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/skullcandy-openid-configuration.json\nnotes:\n- 'Standard Shopify Customer Account API auth: OIDC authorization-code flow with\n  PKCE (S256). The customer-account-mcp-api:full scope grants a customer-scoped\n  MCP surface.'\n- 'Agentic UCP checkout (mcp/skullcandy-mcp.yml) does not require customer login\n  for catalog/cart operations; payment is authorized per-transaction through the\n  registered payment handlers with human approval.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skullcandy/refs/heads/main/authentication/skullcandy-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer Electronics
- Audio
- Headphones
- E-Commerce
- Retail
- Shopify
- Agentic Commerce
- MCP
- Universal Commerce Protocol
---
