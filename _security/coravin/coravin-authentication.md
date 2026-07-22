---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Coravin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coravin secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coravin
provider_slug: coravin
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://shopify.com/authentication/83805208849/oauth/authorize
    endSessionUrl: https://shopify.com/authentication/83805208849/logout
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/83805208849/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/83805208849
  jwks_uri: https://shopify.com/authentication/83805208849/.well-known/jwks.json
  name: ShopifyCustomerAccounts
  openIdConnectUrl: https://www.coravin.com/.well-known/openid-configuration
  sources:
  - well-known/coravin-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: coravin-authentication
source_filename: coravin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.coravin.com/.well-known/openid-configuration\nnotes: >-\n  Auth model captured from the live OIDC / OAuth 2.0 authorization-server\n  metadata published by Coravin's Shopify storefront (Shopify Customer\n  Accounts). This governs customer-account and agentic-commerce access, not a\n  standalone Coravin developer API (Coravin publishes none).\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\nschemes:\n  - name: ShopifyCustomerAccounts\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/83805208849\n    openIdConnectUrl: https://www.coravin.com/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/83805208849/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/83805208849/oauth/token\n        endSessionUrl: https://shopify.com/authentication/83805208849/logout\n\
  \    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    token_endpoint_auth_methods: [client_secret_basic]\n    code_challenge_methods: [S256]\n    jwks_uri: https://shopify.com/authentication/83805208849/.well-known/jwks.json\n    sources: [well-known/coravin-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coravin/refs/heads/main/authentication/coravin-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Wine
- Beverage
- Consumer Products
- Ecommerce
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Wine Preservation
---
