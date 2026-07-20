---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hawthorne Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refresh_token
- jwt-bearer
overview: Hawthorne secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refresh_token, and jwt-bearer flow(s).
provider_name: Hawthorne
provider_slug: hawthorne
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/57105744010/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/57105744010/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/57105744010
  jwks_uri: https://shopify.com/authentication/57105744010/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://hawthorne.co/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/hawthorne-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/57105744010/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: hawthorne-authentication
source_filename: hawthorne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://hawthorne.co/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Authentication is provided by Shopify's Customer Account API for this store\n  (OpenID Connect). Discovery metadata is served from the store host at\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server;\n  the issuer is Shopify (shopify.com/authentication/57105744010). PKCE (S256) is\n  supported. There is no separate first-party Hawthorne developer API auth surface.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refresh_token, jwt-bearer]\n  pkce: [S256]\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/57105744010\n  openIdConnectUrl: https://hawthorne.co/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/57105744010/oauth/authorize\n  token_endpoint:\
  \ https://shopify.com/authentication/57105744010/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/57105744010/logout\n  jwks_uri: https://shopify.com/authentication/57105744010/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources: [well-known/hawthorne-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawthorne/refs/heads/main/authentication/hawthorne-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- E-Commerce
- Retail
- Consumer Goods
- Personal Care
- Grooming
- Agentic Commerce
- Shopify
---
