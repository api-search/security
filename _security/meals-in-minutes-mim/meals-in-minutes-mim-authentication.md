---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Meals In Minutes Mim Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Meals In Minutes, MIM secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Meals In Minutes, MIM
provider_slug: meals-in-minutes-mim
scheme_count: 1
schemes:
- authorization_endpoint: https://account.mealsinminutes.co/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.mealsinminutes.co/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/93906960748
  jwks_uri: https://account.mealsinminutes.co/authentication/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://mealsinminutes.co/.well-known/openid-configuration
  response_types:
  - code
  sources:
  - well-known/meals-in-minutes-mim-openid-configuration.json
  token_endpoint: https://account.mealsinminutes.co/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: meals-in-minutes-mim-authentication
source_filename: meals-in-minutes-mim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mealsinminutes.co/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  notes: >-\n    Shopify Customer Accounts OpenID Connect. Buyer/customer authentication only —\n    the storefront ships no independent developer API key program. Agent commerce\n    via the UCP MCP endpoint is buyer-approval gated, not API-key gated.\nschemes:\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/93906960748\n  openIdConnectUrl: https://mealsinminutes.co/.well-known/openid-configuration\n  authorization_endpoint: https://account.mealsinminutes.co/authentication/oauth/authorize\n  token_endpoint: https://account.mealsinminutes.co/authentication/oauth/token\n  end_session_endpoint: https://account.mealsinminutes.co/authentication/logout\n  jwks_uri: https://account.mealsinminutes.co/authentication/.well-known/jwks.json\n\
  \  response_types: [code]\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  code_challenge_methods: [S256]\n  sources: [well-known/meals-in-minutes-mim-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meals-in-minutes-mim/refs/heads/main/authentication/meals-in-minutes-mim-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Food and Beverage
- Meal Delivery
- E-Commerce
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
---
