---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pair Eyewear Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Pair Eyewear secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Pair Eyewear
provider_slug: pair-eyewear
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/11479910/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/11479910/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/11479910
  jwks_uri: https://shopify.com/authentication/11479910/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://paireyewear.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/pair-eyewear-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/11479910/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: pair-eyewear-authentication
source_filename: pair-eyewear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://paireyewear.com/.well-known/openid-configuration\ndocs: https://paireyewear.com/agents.md\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, refreshToken]\n  notes: >-\n    Customer-facing authentication is provided by Shopify Customer Accounts (OpenID Connect).\n    Agent read/browse of the storefront and UCP discovery require no authentication; UCP/MCP\n    checkout requires contemporaneous buyer approval rather than an API credential.\nschemes:\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://paireyewear.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/11479910\n  authorization_endpoint: https://shopify.com/authentication/11479910/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/11479910/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/11479910/logout\n  jwks_uri:\
  \ https://shopify.com/authentication/11479910/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/pair-eyewear-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pair-eyewear/refs/heads/main/authentication/pair-eyewear-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Eyewear
- Ecommerce
- Retail
- Shopify
- Direct-to-Consumer
- Agent Commerce
- MCP
- UCP
---
