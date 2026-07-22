---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: The Honest Company Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: The Honest Company secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: The Honest Company
provider_slug: the-honest-company
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/64768475320/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/64768475320/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/64768475320
  jwks_uri: https://shopify.com/authentication/64768475320/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.honest.com/.well-known/openid-configuration
  response_types:
  - code
  sources:
  - well-known/the-honest-company-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/64768475320/oauth/token
  type: openIdConnect
slug: the-honest-company-authentication
source_filename: the-honest-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.honest.com/.well-known/openid-configuration\nnotes: >-\n  Derived from the live OpenID Connect discovery document served at\n  www.honest.com/.well-known/openid-configuration. The storefront is powered by\n  Shopify; authentication is Shopify's Customer Account API (issuer\n  https://shopify.com/authentication/64768475320), not a first-party Honest\n  Company developer API.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.honest.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/64768475320\n  authorization_endpoint: https://shopify.com/authentication/64768475320/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/64768475320/oauth/token\n  end_session_endpoint:\
  \ https://shopify.com/authentication/64768475320/logout\n  jwks_uri: https://shopify.com/authentication/64768475320/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  id_token_signing_alg:\n  - RS256\n  sources:\n  - well-known/the-honest-company-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-honest-company/refs/heads/main/authentication/the-honest-company-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Consumer Goods
- Ecommerce
- Retail
- Baby
- Personal Care
- Shopify
---
