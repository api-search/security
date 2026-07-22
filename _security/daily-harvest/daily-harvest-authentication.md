---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Daily Harvest Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Daily Harvest secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Daily Harvest
provider_slug: daily-harvest
scheme_count: 1
schemes:
- authorizationUrl: https://account.daily-harvest.com/authentication/oauth/authorize
  endSessionUrl: https://account.daily-harvest.com/authentication/logout
  issuer: https://shopify.com/authentication/73275670826
  jwksUri: https://account.daily-harvest.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oidc
  responseTypes:
  - code
  sources:
  - well-known/daily-harvest-openid-configuration.json
  tokenEndpointAuthMethods:
  - client_secret_basic
  tokenUrl: https://account.daily-harvest.com/authentication/oauth/token
  type: openIdConnect
slug: daily-harvest-authentication
source_filename: daily-harvest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://daily-harvest.com/.well-known/openid-configuration\nnote: >-\n  Derived from the live OIDC discovery document served on the provider host.\n  This is the Shopify Customer Account API authorization surface for\n  account.daily-harvest.com — Daily Harvest publishes no first-party developer\n  API. Captured for completeness of the provider's public auth surface.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: [S256]\n  id_token_signing: [RS256]\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/73275670826\n  authorizationUrl: https://account.daily-harvest.com/authentication/oauth/authorize\n  tokenUrl: https://account.daily-harvest.com/authentication/oauth/token\n  endSessionUrl: https://account.daily-harvest.com/authentication/logout\n\
  \  jwksUri: https://account.daily-harvest.com/authentication/.well-known/jwks.json\n  responseTypes: [code]\n  tokenEndpointAuthMethods: [client_secret_basic]\n  sources: [well-known/daily-harvest-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daily-harvest/refs/heads/main/authentication/daily-harvest-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Food & Beverage
- Direct-to-Consumer
- E-commerce
- Food Delivery
- Health & Wellness
- Subscription
- Shopify
---
