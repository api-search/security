---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Rouje Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rouje secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rouje
provider_slug: rouje
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/69929140544/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/69929140544/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/69929140544
  jwks_uri: https://shopify.com/authentication/69929140544/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.rouje.com/.well-known/openid-configuration
  sources:
  - well-known/rouje-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/69929140544/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: rouje-authentication
source_filename: rouje-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.rouje.com/.well-known/openid-configuration\nnote: >-\n  Rouje has no first-party developer API. Authentication is provided by the\n  Shopify Customer Account API (OpenID Connect) fronting the storefront, and by\n  the buyer-approval flow of the Universal Commerce Protocol for agent commerce.\n  Read-only catalog browsing (/products/{handle}.json, /collections/*) requires\n  no authentication.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  api_key_in: []\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.rouje.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/69929140544\n  authorization_endpoint: https://shopify.com/authentication/69929140544/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/69929140544/oauth/token\n  jwks_uri: https://shopify.com/authentication/69929140544/.well-known/jwks.json\n\
  \  end_session_endpoint: https://shopify.com/authentication/69929140544/logout\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  sources: [well-known/rouje-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rouje/refs/heads/main/authentication/rouje-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Fashion
- Beauty
- Retail
- Ecommerce
- Shopify
- Agentic Commerce
- Paris
---
