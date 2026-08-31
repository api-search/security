---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Tamara Mellon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tamara Mellon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tamara Mellon
provider_slug: tamara-mellon
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/11034464/oauth/authorize
  bearer_methods_supported:
  - header
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  end_session_endpoint: https://shopify.com/authentication/11034464/logout
  first_party: false
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_account_oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/11034464
  jwks_uri: https://shopify.com/authentication/11034464/.well-known/jwks.json
  openid_configuration: https://shop.tamaramellon.com/.well-known/openid-configuration
  operator: Shopify
  pkce:
    required_methods:
    - S256
  protected_resource: https://shop.tamaramellon.com
  response_types:
  - code
  token_endpoint: https://shopify.com/authentication/11034464/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: tamara-mellon-authentication
source_filename: tamara-mellon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://shop.tamaramellon.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary: >-\n  Tamara Mellon publishes no first-party API and therefore no first-party authentication model. The\n  only authentication surface reachable on a host the company controls is the Shopify Customer Account\n  OAuth 2.0 / OpenID Connect provider that Shopify mounts for every storefront, discovered at\n  shop.tamaramellon.com/.well-known/openid-configuration and scoped to this shop (id 11034464). It\n  authenticates the brand's own retail customers into their account; it is not a developer-facing API\n  credential surface, and no client registration, key issuance, or developer program exists.\nfirst_party_api: false\nschemes:\n- id: shopify_customer_account_oidc\n  type: openIdConnect\n  first_party: false\n  operator: Shopify\n  openid_configuration: https://shop.tamaramellon.com/.well-known/openid-configuration\n\
  \  issuer: https://shopify.com/authentication/11034464\n  authorization_endpoint: https://shopify.com/authentication/11034464/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/11034464/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/11034464/logout\n  jwks_uri: https://shopify.com/authentication/11034464/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n    required_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  bearer_methods_supported:\n  - header\n  protected_resource: https://shop.tamaramellon.com\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\nnotes:\n- The store is password-gated, so the authorization endpoints cannot be exercised end to end.\n- No API keys, no personal\
  \ access tokens, no developer application registration is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamara-mellon/refs/heads/main/authentication/tamara-mellon-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fashion
- Footwear
- Luxury
- Retail
- Direct to Consumer
- E-Commerce
- Consumer Goods
- Apparel
---
