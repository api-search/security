---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Honest Company Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: Honest Company secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: Honest Company
provider_slug: honest-company
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/64768475320/oauth/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/64768475320
  jwks_uri: https://shopify.com/authentication/64768475320/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://honest.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/honest-company-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/64768475320/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: honest-company-authentication
source_filename: honest-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://honest.com/.well-known/openid-configuration\ndocs: https://honest.com/account/login\nnotes: >-\n  Derived from the live OIDC discovery document served at honest.com. The\n  storefront authenticates shoppers via the Shopify Customer Account API, an\n  OAuth2 / OpenID Connect authorization server. No first-party OpenAPI is\n  published, so this profile is transcribed from the discovery document rather\n  than from securitySchemes.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - jwtBearer\n  pkce: S256\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://honest.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/64768475320\n  authorization_endpoint: https://shopify.com/authentication/64768475320/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/64768475320/oauth/token\n\
  \  jwks_uri: https://shopify.com/authentication/64768475320/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  sources:\n  - well-known/honest-company-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honest-company/refs/heads/main/authentication/honest-company-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer Goods
- E-commerce
- Retail
- Baby Care
- Personal Care
- Beauty
- Shopify
- Agentic Commerce
- MCP
- UCP
---
