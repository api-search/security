---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Allbirds Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Allbirds secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Allbirds
provider_slug: allbirds
scheme_count: 1
schemes:
- authorizationUrl: https://accounts.allbirds.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  endSessionUrl: https://accounts.allbirds.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/11044168
  jwksUri: https://accounts.allbirds.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.allbirds.com/.well-known/openid-configuration
  sources:
  - well-known/allbirds-openid-configuration.json
  tokenUrl: https://accounts.allbirds.com/authentication/oauth/token
  type: openIdConnect
slug: allbirds-authentication
source_filename: allbirds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.allbirds.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  No first-party OpenAPI is published, so this profile is read from Allbirds's\n  live OIDC / OAuth 2.0 authorization-server discovery documents. Authentication\n  is Shopify Customer Accounts: OpenID Connect + OAuth 2.0 Authorization Code\n  with PKCE. The storefront/UCP MCP read tools need no auth; transacting requires\n  buyer-approved authorization.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: S256\n  token_endpoint_auth: [client_secret_basic]\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/11044168\n    openIdConnectUrl: https://www.allbirds.com/.well-known/openid-configuration\n    authorizationUrl: https://accounts.allbirds.com/authentication/oauth/authorize\n  \
  \  tokenUrl: https://accounts.allbirds.com/authentication/oauth/token\n    endSessionUrl: https://accounts.allbirds.com/authentication/logout\n    jwksUri: https://accounts.allbirds.com/authentication/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    code_challenge_methods: [S256]\n    sources: [well-known/allbirds-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allbirds/refs/heads/main/authentication/allbirds-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Retail
- E-commerce
- Footwear
- Apparel
- Sustainability
- Direct-to-Consumer
- Agent Commerce
- Shopify
---
