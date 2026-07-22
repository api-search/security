---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jinx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jinx secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jinx
provider_slug: jinx
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/27716059229/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/27716059229/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/27716059229
  jwks_uri: https://shopify.com/authentication/27716059229/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://thinkjinx.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/jinx-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/27716059229/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: jinx-authentication
source_filename: jinx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://thinkjinx.com/.well-known/openid-configuration\nnote: >-\n  Jinx has no first-party public API. The only machine authentication surface is\n  the Shopify Customer Account API, whose OIDC/OAuth discovery is served live from\n  the storefront (issuer scoped to shop id 27716059229). Captured from the\n  well-known discovery document, not from an OpenAPI spec.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  provider: shopify-customer-account-api\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://thinkjinx.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/27716059229\n  authorization_endpoint: https://shopify.com/authentication/27716059229/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/27716059229/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/27716059229/logout\n\
  \  jwks_uri: https://shopify.com/authentication/27716059229/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  sources: [well-known/jinx-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jinx/refs/heads/main/authentication/jinx-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Pet Food
- Pet Nutrition
- Ecommerce
- Direct to Consumer
- Dogs
- Cats
- Shopify
---
