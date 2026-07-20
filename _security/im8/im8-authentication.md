---
api_key_in: []
auth_types: []
description: Authentication profile for the IM8 Health storefront's buyer-scoped APIs, derived from the store's Shopify Customer Account OpenID Connect / OAuth 2.0 discovery documents. Read-only catalog browsing (product/collection JSON, search) requires no authentication; account- and purchase-scoped operations use OAuth 2.0 Authorization Code with PKCE.
kind: authentication
layout: security
method: searched
name: Im8 Authentication
name_suffix: Authentication
oauth_flows: []
overview: IM8 Health declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: IM8 Health
provider_slug: im8
scheme_count: 2
schemes:
- authorization_endpoint: https://account.im8health.com/authentication/oauth/authorize
  end_session_endpoint: https://account.im8health.com/authentication/logout
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/63744606375
  jwks_uri: https://account.im8health.com/authentication/.well-known/jwks.json
  name: shopify_customer_account_oauth2
  pkce: true
  pkce_methods:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://account.im8health.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
- description: Read-only storefront browsing (collections, product JSON, search) needs no auth.
  name: none
  type: none
slug: im8-authentication
source_filename: im8-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://im8health.com/.well-known/openid-configuration\ntype: Authentication\ndescription: >-\n  Authentication profile for the IM8 Health storefront's buyer-scoped APIs, derived\n  from the store's Shopify Customer Account OpenID Connect / OAuth 2.0 discovery\n  documents. Read-only catalog browsing (product/collection JSON, search) requires\n  no authentication; account- and purchase-scoped operations use OAuth 2.0\n  Authorization Code with PKCE.\nschemes:\n- name: shopify_customer_account_oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce: true\n  pkce_methods:\n  - S256\n  issuer: https://shopify.com/authentication/63744606375\n  authorization_endpoint: https://account.im8health.com/authentication/oauth/authorize\n  token_endpoint: https://account.im8health.com/authentication/oauth/token\n  end_session_endpoint: https://account.im8health.com/authentication/logout\n  jwks_uri: https://account.im8health.com/authentication/.well-known/jwks.json\n\
  \  token_endpoint_auth_methods:\n  - client_secret_basic\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n- name: none\n  type: none\n  description: Read-only storefront browsing (collections, product JSON, search) needs no auth.\nnotes:\n- OpenID Connect is supported (openid scope, id_token RS256, standard OIDC claims).\n- customer-account-mcp-api:full scope authorizes MCP-driven access to customer account data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/im8/refs/heads/main/authentication/im8-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Health
- Wellness
- Supplements
- Nutrition
- Ecommerce
- Direct-to-Consumer
- Agentic Commerce
- Shopify
- UCP
- MCP
---
