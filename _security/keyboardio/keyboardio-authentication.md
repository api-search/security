---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Keyboardio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Keyboardio secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Keyboardio
provider_slug: keyboardio
scheme_count: 1
schemes:
- authorization_endpoint: https://account.keyboard.io/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.keyboard.io/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/9200728
  jwks_uri: https://account.keyboard.io/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://keyboard.io/.well-known/openid-configuration
  sources:
  - well-known/keyboardio-openid-configuration.json
  token_endpoint: https://account.keyboard.io/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: keyboardio-authentication
source_filename: keyboardio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://keyboard.io/.well-known/openid-configuration\ndocs: https://keyboard.io/.well-known/openid-configuration\nnote: >-\n  Keyboardio has no first-party HTTP API. The only auth surface on the domain\n  is Shopify Customer Accounts (OpenID Connect / OAuth 2.0) bound to\n  keyboard.io, used for customer login and the Shopify Customer Account API.\n  Issuer https://shopify.com/authentication/9200728; endpoints hosted at\n  account.keyboard.io.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://keyboard.io/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/9200728\n  authorization_endpoint: https://account.keyboard.io/authentication/oauth/authorize\n  token_endpoint: https://account.keyboard.io/authentication/oauth/token\n  end_session_endpoint: https://account.keyboard.io/authentication/logout\n\
  \  jwks_uri: https://account.keyboard.io/authentication/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  sources:\n  - well-known/keyboardio-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyboardio/refs/heads/main/authentication/keyboardio-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Mechanical Keyboards
- Hardware
- Ergonomics
- Open Source
- Firmware
- Keyboards
- E-commerce
---
