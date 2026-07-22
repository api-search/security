---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Byheart Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ByHeart secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ByHeart
provider_slug: byheart
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/59458650296/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/59458650296/logout
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/59458650296
  jwks_uri: https://shopify.com/authentication/59458650296/.well-known/jwks.json
  name: shopifyCustomerAccountOIDC
  provider: Shopify Customer Account API
  sources:
  - well-known/byheart-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/59458650296/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: byheart-authentication
source_filename: byheart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.byheart.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  ByHeart's storefront authenticates customers via Shopify's Customer Account\n  API, an OpenID Connect / OAuth 2.0 authorization server hosted by Shopify and\n  advertised under the ByHeart domain. There is no first-party ByHeart API.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\nschemes:\n- name: shopifyCustomerAccountOIDC\n  type: openIdConnect\n  provider: Shopify Customer Account API\n  issuer: https://shopify.com/authentication/59458650296\n  authorization_endpoint: https://shopify.com/authentication/59458650296/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/59458650296/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/59458650296/logout\n\
  \  jwks_uri: https://shopify.com/authentication/59458650296/.well-known/jwks.json\n  id_token_signing_alg: [RS256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  code_challenge_methods: [S256]\n  sources: [well-known/byheart-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byheart/refs/heads/main/authentication/byheart-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Infant Nutrition
- Baby Formula
- Direct-to-Consumer
- Ecommerce
- Health
- Shopify
---
