---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Casper Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Casper secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Casper
provider_slug: casper
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/60822683729/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/60822683729/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/60822683729
  jwks_uri: https://shopify.com/authentication/60822683729/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://casper.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/casper-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/60822683729/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: casper-authentication
source_filename: casper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://casper.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  casper.com is a Shopify storefront. Customer-facing authentication is the Shopify\n  Customer Account API using OpenID Connect / OAuth 2.0 (authorization code + PKCE).\n  Anonymous read-only browsing (product/collection JSON) requires no auth.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: true\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/60822683729\n  openIdConnectUrl: https://casper.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/60822683729/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/60822683729/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/60822683729/logout\n  jwks_uri:\
  \ https://shopify.com/authentication/60822683729/.well-known/jwks.json\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  sources: [well-known/casper-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casper/refs/heads/main/authentication/casper-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Ecommerce
- Retail
- Sleep
- Mattresses
- Direct to Consumer
- Agentic Commerce
- Shopify
---
