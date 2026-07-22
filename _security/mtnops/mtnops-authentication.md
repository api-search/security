---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Mtnops Authentication
name_suffix: Authentication
oauth_flows: []
overview: MTN OPS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MTN OPS
provider_slug: mtnops
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/27864584/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/27864584/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/27864584
  jwks_uri: https://shopify.com/authentication/27864584/.well-known/jwks.json
  name: shopify-customer-accounts
  openid_configuration: https://mtnops.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/27864584/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: mtnops-authentication
source_filename: mtnops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mtnops.com/.well-known/openid-configuration\nnote: >-\n  MTN OPS is a Shopify storefront. Customer-facing authentication is handled by\n  Shopify New Customer Accounts via OpenID Connect / OAuth 2.0. The values below\n  are read verbatim from the live OIDC discovery document on the mtnops.com\n  domain. There is no separate MTN OPS developer API auth surface.\nschemes:\n- type: openIdConnect\n  name: shopify-customer-accounts\n  issuer: https://shopify.com/authentication/27864584\n  openid_configuration: https://mtnops.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/27864584/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/27864584/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/27864584/logout\n  jwks_uri: https://shopify.com/authentication/27864584/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n\
  \  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - S256\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mtnops/refs/heads/main/authentication/mtnops-authentication.yml
summary_line: 1 scheme
tags:
- Company
- E-commerce
- Retail
- Consumer Products
- Nutrition
- Supplements
- Outdoor
- Shopify
---
