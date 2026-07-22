---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Mori Authentication
name_suffix: Authentication
oauth_flows: []
overview: MORI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MORI
provider_slug: mori
scheme_count: 2
schemes:
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  id_token_signing_alg: RS256
  jwks_status: 200
  jwks_uri: https://shopify.com/authentication/6726617/.well-known/jwks.json
  openIdConnectUrl: https://babymori.com/.well-known/openid-configuration
  type: openIdConnect
- flows:
    authorization_code:
      authorization_endpoint: https://shopify.com/authentication/6726617/oauth/authorize
      code_challenge_methods:
      - S256
      end_session_endpoint: https://shopify.com/authentication/6726617/logout
      pkce: true
      token_endpoint: https://shopify.com/authentication/6726617/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
slug: mori-authentication
source_filename: mori-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: live probe of https://babymori.com/.well-known/openid-configuration and /.well-known/oauth-authorization-server (Shopify Customer Account API)\nnote: >-\n  The only authenticated machine surface on babymori.com is Shopify's Customer\n  Account API for this store, which advertises OpenID Connect + OAuth 2.0\n  discovery. MORI does not operate a first-party auth server; the issuer is\n  Shopify (authentication/6726617). The storefront browsing/cart MCP at\n  /api/mcp requires no authentication.\nissuer: https://shopify.com/authentication/6726617\nschemes:\n- type: openIdConnect\n  openIdConnectUrl: https://babymori.com/.well-known/openid-configuration\n  id_token_signing_alg: RS256\n  jwks_uri: https://shopify.com/authentication/6726617/.well-known/jwks.json\n  jwks_status: 200\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n- type: oauth2\n  flows:\n    authorization_code:\n\
  \      authorization_endpoint: https://shopify.com/authentication/6726617/oauth/authorize\n      token_endpoint: https://shopify.com/authentication/6726617/oauth/token\n      end_session_endpoint: https://shopify.com/authentication/6726617/logout\n      pkce: true\n      code_challenge_methods:\n      - S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\nop_policy_uri: https://www.shopify.com/legal/privacy\nop_tos_uri: https://www.shopify.com/legal/terms\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mori/refs/heads/main/authentication/mori-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Retail
- E-commerce
- Baby Products
- Consumer Goods
- Apparel
- Direct to Consumer
- Shopify
- MCP
- Agent Native
- Universal Commerce Protocol
---
