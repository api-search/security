---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Stance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Stance secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Stance
provider_slug: stance
scheme_count: 1
schemes:
- authorization_endpoint: https://account.stance.com/authentication/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.stance.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/102408782162
  jwks_uri: https://account.stance.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  response_types_supported:
  - code
  sources:
  - well-known/stance-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://account.stance.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: stance-authentication
source_filename: stance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://stance.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Derived from the live OpenID Connect / OAuth 2.0 discovery document served at\n  stance.com. Stance's storefront runs on Shopify; customer authentication is\n  the Shopify Customer Account API (OIDC), with authorization and token\n  endpoints hosted under account.stance.com. This is the only public auth\n  surface for stance.com — the retail storefront itself exposes no product API.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  token_endpoint_auth: client_secret_basic\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/102408782162\n  authorization_endpoint: https://account.stance.com/authentication/oauth/authorize\n  token_endpoint: https://account.stance.com/authentication/oauth/token\n  end_session_endpoint:\
  \ https://account.stance.com/authentication/logout\n  jwks_uri: https://account.stance.com/authentication/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  sources:\n  - well-known/stance-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stance/refs/heads/main/authentication/stance-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Apparel
- Retail
- E-commerce
- Socks
- Direct-to-Consumer
- Shopify
---
