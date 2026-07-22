---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: The Beard Club Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: The Beard Club secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: The Beard Club
provider_slug: the-beard-club
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/5260181607/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/5260181607/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/5260181607
  jwks_uri: https://shopify.com/authentication/5260181607/.well-known/jwks.json
  name: ShopifyCustomerAccount
  openIdConnectUrl: https://thebeardclub.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/the-beard-club-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/5260181607/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: the-beard-club-authentication
source_filename: the-beard-club-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://thebeardclub.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  note: >-\n    Customer-facing auth is Shopify's Customer Account API (OIDC / OAuth 2.0\n    Authorization Code + PKCE). Agent commerce is transacted over the UCP MCP\n    endpoint; checkout completion additionally requires contemporaneous buyer\n    approval. No merchant/admin API key surface is publicly exposed.\nschemes:\n- name: ShopifyCustomerAccount\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/5260181607\n  openIdConnectUrl: https://thebeardclub.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/5260181607/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/5260181607/oauth/token\n  jwks_uri: https://shopify.com/authentication/5260181607/.well-known/jwks.json\n\
  \  end_session_endpoint: https://shopify.com/authentication/5260181607/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/the-beard-club-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-beard-club/refs/heads/main/authentication/the-beard-club-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- E-commerce
- Retail
- Men's Grooming
- Consumer Goods
- Shopify
- Agent Commerce
- UCP
- MCP
- Subscription
---
