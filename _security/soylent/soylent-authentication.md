---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Soylent Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Soylent secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Soylent
provider_slug: soylent
scheme_count: 1
schemes:
- authorizationUrl: https://account.soylent.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  endSessionUrl: https://account.soylent.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values:
  - RS256
  issuer: https://shopify.com/authentication/359333902
  jwksUri: https://account.soylent.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://soylent.com/.well-known/openid-configuration
  sources:
  - well-known/soylent-openid-configuration.json
  tokenUrl: https://account.soylent.com/authentication/oauth/token
  type: openIdConnect
slug: soylent-authentication
source_filename: soylent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://soylent.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  No first-party OpenAPI is published, so this profile is read from Soylent's\n  live OIDC / OAuth 2.0 authorization-server discovery documents. Authentication\n  is Shopify Customer Accounts: OpenID Connect + OAuth 2.0 Authorization Code\n  with PKCE (S256). The storefront / UCP MCP read tools need no auth; transacting\n  requires buyer-approved authorization.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: S256\n  token_endpoint_auth: [client_secret_basic]\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/359333902\n    openIdConnectUrl: https://soylent.com/.well-known/openid-configuration\n    authorizationUrl: https://account.soylent.com/authentication/oauth/authorize\n    tokenUrl:\
  \ https://account.soylent.com/authentication/oauth/token\n    endSessionUrl: https://account.soylent.com/authentication/logout\n    jwksUri: https://account.soylent.com/authentication/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    code_challenge_methods: [S256]\n    id_token_signing_alg_values: [RS256]\n    sources: [well-known/soylent-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soylent/refs/heads/main/authentication/soylent-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Nutrition
- Food and Beverage
- Meal Replacement
- Ecommerce
- Retail
- Direct-to-Consumer
- Agent Commerce
- Universal Commerce Protocol
- Shopify
- MCP
---
