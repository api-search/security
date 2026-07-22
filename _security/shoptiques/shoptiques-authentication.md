---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Shoptiques Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Shoptiques secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Shoptiques
provider_slug: shoptiques
scheme_count: 1
schemes:
- authorization_endpoint: https://account.shoptiques.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.shoptiques.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/70666223927
  jwks_uri: https://account.shoptiques.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://shoptiques.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/shoptiques-openid-configuration.json
  token_endpoint: https://account.shoptiques.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: shoptiques-authentication
source_filename: shoptiques-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://shoptiques.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Shoptiques runs on Shopify. Buyer/customer authentication is the Shopify\n  Customer Account API using OpenID Connect / OAuth 2.0 (authorization code + PKCE).\n  Agentic commerce (UCP) transactions require buyer approval; read-only storefront\n  browsing (product/collection JSON) requires no authentication.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://shoptiques.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/70666223927\n    authorization_endpoint: https://account.shoptiques.com/authentication/oauth/authorize\n    token_endpoint: https://account.shoptiques.com/authentication/oauth/token\n    end_session_endpoint: https://account.shoptiques.com/authentication/logout\n\
  \    jwks_uri: https://account.shoptiques.com/authentication/.well-known/jwks.json\n    response_types_supported: [code]\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - \"urn:ietf:params:oauth:grant-type:jwt-bearer\"\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    id_token_signing_alg_values_supported: [RS256]\n    sources: [well-known/shoptiques-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoptiques/refs/heads/main/authentication/shoptiques-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- E-Commerce
- Retail
- Marketplace
- Boutiques
- Fashion
- Agentic Commerce
- Shopify
- MCP
- UCP
---
