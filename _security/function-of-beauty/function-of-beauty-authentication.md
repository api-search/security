---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Function Of Beauty Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Function of Beauty secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Function of Beauty
provider_slug: function-of-beauty
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/69081399608/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/69081399608/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/69081399608
  jwks_uri: https://shopify.com/authentication/69081399608/.well-known/jwks.json
  name: shopifyCustomerAccount
  openIdConnectUrl: https://functionofbeauty.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/function-of-beauty-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/69081399608/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: function-of-beauty-authentication
source_filename: function-of-beauty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://functionofbeauty.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Function of Beauty is a Shopify-hosted store. Its customer-facing authentication\n  surface is the Shopify Customer Account API, exposed via OpenID Connect discovery\n  on the provider domain. The scheme below is read verbatim from the live\n  openid-configuration document.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\nschemes:\n- name: shopifyCustomerAccount\n  type: openIdConnect\n  openIdConnectUrl: https://functionofbeauty.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/69081399608\n  authorization_endpoint: https://shopify.com/authentication/69081399608/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/69081399608/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/69081399608/logout\n\
  \  jwks_uri: https://shopify.com/authentication/69081399608/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - S256\n  sources:\n  - well-known/function-of-beauty-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/function-of-beauty/refs/heads/main/authentication/function-of-beauty-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Beauty
- Personal Care
- Personalization
- E-Commerce
- Shopify
- Direct to Consumer
- MCP
---
