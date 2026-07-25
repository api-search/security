---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Our Place Authentication
name_suffix: Authentication
oauth_flows: []
overview: Our Place declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Our Place
provider_slug: our-place
scheme_count: 1
schemes:
- authorization_endpoint: https://account.fromourplace.com/authentication/oauth/authorize
  end_session_endpoint: https://account.fromourplace.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/2441379915
  jwks_uri: https://account.fromourplace.com/authentication/.well-known/jwks.json
  name: shopify-customer-account
  openIdConnectUrl: https://fromourplace.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://account.fromourplace.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: our-place-authentication
source_filename: our-place-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://fromourplace.com/.well-known/openid-configuration\nsummary: >-\n  Our Place authenticates customers and agents through Shopify Customer Accounts,\n  an OpenID Connect / OAuth 2.0 provider. The authorization-code flow with PKCE\n  (S256) is used; the customer-account MCP scope gates agentic commerce access.\nschemes:\n- type: openIdConnect\n  name: shopify-customer-account\n  openIdConnectUrl: https://fromourplace.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/2441379915\n  authorization_endpoint: https://account.fromourplace.com/authentication/oauth/authorize\n  token_endpoint: https://account.fromourplace.com/authentication/oauth/token\n  end_session_endpoint: https://account.fromourplace.com/authentication/logout\n  jwks_uri: https://account.fromourplace.com/authentication/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  response_types:\n  - code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  pkce:\n    code_challenge_methods:\n    - S256\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\nnotes:\n- Storefront product/collection JSON is readable without authentication.\n- Agentic checkout via the UCP MCP endpoint still requires buyer payment approval.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/our-place/refs/heads/main/authentication/our-place-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Ecommerce
- Retail
- Cookware
- Consumer
- Agentic Commerce
- Shopify
---
