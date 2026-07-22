---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Shopshops Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ShopShops secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ShopShops
provider_slug: shopshops
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/59001897017/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/59001897017/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/59001897017
  jwks_uri: https://shopify.com/authentication/59001897017/.well-known/jwks.json
  name: CustomerAccountOIDC
  response_types_supported:
  - code
  sources:
  - well-known/shopshops-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/59001897017/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: shopshops-authentication
source_filename: shopshops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.shopshopslive.com/.well-known/openid-configuration\ndocs: https://www.shopshopslive.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  note: >-\n    ShopShops (on Shopify) exposes an OIDC/OAuth2 Customer Account API for\n    authenticated buyer access. Agent commerce runs over the UCP MCP endpoint,\n    where checkout requires contemporaneous buyer payment approval.\nschemes:\n- name: CustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/59001897017\n  authorization_endpoint: https://shopify.com/authentication/59001897017/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/59001897017/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/59001897017/logout\n  jwks_uri: https://shopify.com/authentication/59001897017/.well-known/jwks.json\n  response_types_supported:\
  \ [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [S256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources: [well-known/shopshops-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopshops/refs/heads/main/authentication/shopshops-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Commerce
- Ecommerce
- Marketplace
- Live Shopping
- Luxury Resale
- Agent Commerce
- Shopify
---
