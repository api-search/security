---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Zulily Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refresh_token
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: Zulily secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refresh_token, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: Zulily
provider_slug: zulily
scheme_count: 1
schemes:
- authorization_endpoint: https://account.zulily.com/authentication/oauth/authorize
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.zulily.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/4710885
  jwks_uri: https://account.zulily.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccount
  provider: Shopify Customer Account API
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/zulily-openid-configuration.json
  token_endpoint: https://account.zulily.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: zulily-authentication
source_filename: zulily-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.zulily.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: S256\n  token_endpoint_auth: client_secret_basic\nschemes:\n  - name: ShopifyCustomerAccount\n    type: openIdConnect\n    provider: Shopify Customer Account API\n    issuer: https://shopify.com/authentication/4710885\n    authorization_endpoint: https://account.zulily.com/authentication/oauth/authorize\n    token_endpoint: https://account.zulily.com/authentication/oauth/token\n    end_session_endpoint: https://account.zulily.com/authentication/logout\n    jwks_uri: https://account.zulily.com/authentication/.well-known/jwks.json\n    id_token_signing_alg: RS256\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    token_endpoint_auth_methods:\
  \ [client_secret_basic]\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    sources: [well-known/zulily-openid-configuration.json]\nnotes: >-\n  Zulily (relaunched on Shopify) authenticates customers via the Shopify Customer Account API using\n  OpenID Connect + OAuth 2.0 authorization-code flow with PKCE (S256). A dedicated\n  customer-account-mcp-api:full scope authorizes agent/MCP access to the customer account surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zulily/refs/heads/main/authentication/zulily-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Ecommerce
- Retail
- Shopping
- Commerce
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
