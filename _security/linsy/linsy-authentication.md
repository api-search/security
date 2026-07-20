---
api_key_in: []
auth_types: []
description: Linsy's authenticated surface is the Shopify customer account system. Each storefront publishes an OpenID Connect discovery document (and an identical RFC 8414 OAuth authorization server metadata document) pointing at a per-shop issuer on shopify.com. Authorization Code with PKCE (S256) is the supported flow; tokens are also obtainable via refresh_token and JWT bearer grants. The anonymous UCP/MCP commerce surface requires no credential — authentication is only involved once a buyer account or a buyer-approved payment is in play.
kind: authentication
layout: security
method: searched
name: Linsy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linsy declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Linsy
provider_slug: linsy
scheme_count: 3
schemes:
- authorization_endpoint: https://shopify.com/authentication/55555752076/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/55555752076/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_account_oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/55555752076
  jwks_uri: https://shopify.com/authentication/55555752076/.well-known/jwks.json
  openIdConnectUrl: https://www.linsyhome.com/.well-known/openid-configuration
  response_types_supported:
  - code
  store: LINSY HOME
  storefront: https://www.linsyhome.com/
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/55555752076/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- authorization_endpoint: https://shopify.com/authentication/73791996150/oauth/authorize
  code_challenge_methods_supported:
  - S256
  id: shopify_customer_account_oidc_official
  issuer: https://shopify.com/authentication/73791996150
  openIdConnectUrl: https://linsy.com/.well-known/openid-configuration
  response_types_supported:
  - code
  store: Linsy Official Store
  storefront: https://linsy.com/
  token_endpoint: https://shopify.com/authentication/73791996150/oauth/token
  type: openIdConnect
- description: The UCP/MCP commerce endpoint accepts unauthenticated JSON-RPC calls for catalog search, lookup and cart operations. It requires a UCP agent profile URI rather than an API key; calls without one are rejected with JSON-RPC error -32001 (invalid_profile_url). Payment completion is gated on contemporaneous buyer approval, not on an agent credential.
  endpoints:
  - https://www.linsyhome.com/api/ucp/mcp
  - https://linsy.com/api/ucp/mcp
  id: ucp_mcp_anonymous
  type: none
slug: linsy-authentication
source_filename: linsy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.linsyhome.com/.well-known/openid-configuration and https://linsy.com/.well-known/openid-configuration\nname: Linsy authentication profile\ndescription: Linsy's authenticated surface is the Shopify customer account system. Each storefront\n  publishes an OpenID Connect discovery document (and an identical RFC 8414 OAuth authorization server\n  metadata document) pointing at a per-shop issuer on shopify.com. Authorization Code with PKCE (S256)\n  is the supported flow; tokens are also obtainable via refresh_token and JWT bearer grants. The\n  anonymous UCP/MCP commerce surface requires no credential — authentication is only involved once a\n  buyer account or a buyer-approved payment is in play.\nschemes:\n- id: shopify_customer_account_oidc\n  type: openIdConnect\n  store: LINSY HOME\n  storefront: https://www.linsyhome.com/\n  openIdConnectUrl: https://www.linsyhome.com/.well-known/openid-configuration\n  issuer:\
  \ https://shopify.com/authentication/55555752076\n  authorization_endpoint: https://shopify.com/authentication/55555752076/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/55555752076/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/55555752076/logout\n  jwks_uri: https://shopify.com/authentication/55555752076/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n- id: shopify_customer_account_oidc_official\n  type: openIdConnect\n  store: Linsy Official Store\n  storefront: https://linsy.com/\n  openIdConnectUrl:\
  \ https://linsy.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/73791996150\n  authorization_endpoint: https://shopify.com/authentication/73791996150/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/73791996150/oauth/token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n- id: ucp_mcp_anonymous\n  type: none\n  description: The UCP/MCP commerce endpoint accepts unauthenticated JSON-RPC calls for catalog search,\n    lookup and cart operations. It requires a UCP agent profile URI rather than an API key; calls without\n    one are rejected with JSON-RPC error -32001 (invalid_profile_url). Payment completion is gated on\n    contemporaneous buyer approval, not on an agent credential.\n  endpoints:\n  - https://www.linsyhome.com/api/ucp/mcp\n  - https://linsy.com/api/ucp/mcp\nnotes:\n- No first-party developer API keys, no API key registration, and no partner/developer portal are\n  published on either\
  \ Linsy host.\n- op_policy_uri and op_tos_uri on both issuers point at Shopify's platform legal pages, confirming the\n  identity provider is Shopify rather than Linsy-operated.\nrelated:\n  scopes: ../scopes/linsy-scopes.yml\n  well_known: ../well-known/linsy-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linsy/refs/heads/main/authentication/linsy-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Furniture
- Home Goods
- Direct To Consumer
- Agentic Commerce
- Shopify
- MCP
---
