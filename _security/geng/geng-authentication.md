---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Geng Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Gen.G secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Gen.G
provider_slug: geng
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/55492378809/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/55492378809/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/55492378809
  jwks_uri: https://shopify.com/authentication/55492378809/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://geng.gg/.well-known/openid-configuration
  sources:
  - well-known/geng-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/55492378809/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: geng-authentication
source_filename: geng-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://geng.gg/.well-known/openid-configuration\nnotes: >-\n  Auth surface for the geng.gg (Shopify-powered) storefront, described by the\n  Shopify Customer Account API OpenID Connect discovery document served under\n  the geng.gg domain. Gen.G itself publishes no first-party developer API; this\n  is the customer-account authentication for the merch store.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: [S256]\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://geng.gg/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/55492378809\n    authorization_endpoint: https://shopify.com/authentication/55492378809/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/55492378809/oauth/token\n\
  \    end_session_endpoint: https://shopify.com/authentication/55492378809/logout\n    jwks_uri: https://shopify.com/authentication/55492378809/.well-known/jwks.json\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    sources: [well-known/geng-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geng/refs/heads/main/authentication/geng-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Esports
- Gaming
- Entertainment
- Media
- Sports
---
