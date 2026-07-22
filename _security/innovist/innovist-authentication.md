---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Innovist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Innovist secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Innovist
provider_slug: innovist
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/3960733763/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/3960733763/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/3960733763
  jwks_uri: https://shopify.com/authentication/3960733763/.well-known/jwks.json
  name: shopifyCustomerAccountOIDC
  response_types_supported:
  - code
  sources:
  - well-known/innovist-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/3960733763/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: innovist-authentication
source_filename: innovist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://innovist.com/.well-known/openid-configuration\ndocs: https://innovist.com/.well-known/oauth-authorization-server\nnotes: >-\n  Auth profile captured verbatim from the store's live OpenID Connect / OAuth\n  Authorization Server discovery documents (Shopify customer-account identity,\n  issuer https://shopify.com/authentication/3960733763). Covers customer-account\n  sign-in and the customer-account MCP API used for agent commerce.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  id_token_signing_alg:\n  - RS256\nschemes:\n- name: shopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/3960733763\n  authorization_endpoint: https://shopify.com/authentication/3960733763/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/3960733763/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/3960733763/logout\n\
  \  jwks_uri: https://shopify.com/authentication/3960733763/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  sources:\n  - well-known/innovist-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovist/refs/heads/main/authentication/innovist-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Personal Care
- Skincare
- Haircare
- Suncare
- Direct to Consumer
- Ecommerce
- Shopify
- Agentic Commerce
---
