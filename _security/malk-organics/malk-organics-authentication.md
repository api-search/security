---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Malk Organics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: MALK Organics secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: MALK Organics
provider_slug: malk-organics
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/64317849670/oauth/authorize
  code_challenge_methods:
  - S256
  endSessionUrl: https://shopify.com/authentication/64317849670/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/64317849670
  jwksUri: https://shopify.com/authentication/64317849670/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://malkorganics.com/.well-known/openid-configuration
  sources:
  - well-known/malk-organics-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/64317849670/oauth/token
  type: openIdConnect
slug: malk-organics-authentication
source_filename: malk-organics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://malkorganics.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  MALK Organics publishes no OpenAPI, so this profile is read from the live OIDC / OAuth 2.0\n  authorization-server and protected-resource discovery documents served on malkorganics.com.\n  Authentication is Shopify Customer Accounts - OpenID Connect over OAuth 2.0 Authorization\n  Code with PKCE (S256). The UCP/MCP catalog and cart tools answer anonymously; completing a\n  checkout requires contemporaneous buyer approval, and the Customer Account surfaces require\n  a signed-in buyer token.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: S256\n  token_endpoint_auth: [client_secret_basic, client_secret_post]\n  anonymous_surface: >-\n    MCP tools/list and the catalog/cart tools returned HTTP 200 with no credentials.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n\
  \  type: openIdConnect\n  issuer: https://shopify.com/authentication/64317849670\n  openIdConnectUrl: https://malkorganics.com/.well-known/openid-configuration\n  authorizationUrl: https://shopify.com/authentication/64317849670/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/64317849670/oauth/token\n  endSessionUrl: https://shopify.com/authentication/64317849670/logout\n  jwksUri: https://shopify.com/authentication/64317849670/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  sources: [well-known/malk-organics-openid-configuration.json]\nprotected_resource:\n  resource: https://malkorganics.com\n  authorization_servers:\n  - https://shopify.com/authentication/64317849670\n  bearer_methods_supported: [header]\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  sources: [well-known/malk-organics-oauth-protected-resource.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/malk-organics/refs/heads/main/authentication/malk-organics-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Food and Beverage
- Consumer Packaged Goods
- Plant-Based
- Organic
- Direct to Consumer
- Agent Commerce
- MCP
- Shopify
---
