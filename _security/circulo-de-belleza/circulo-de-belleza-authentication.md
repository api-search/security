---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Circulo De Belleza Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Circulo de Belleza secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Circulo de Belleza
provider_slug: circulo-de-belleza
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/25099010151/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/25099010151/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/25099010151
  jwks_uri: https://shopify.com/authentication/25099010151/.well-known/jwks.json
  name: ShopifyCustomerAccountsOIDC
  openIdConnectUrl: https://www.circulodebelleza.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/circulo-de-belleza-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/25099010151/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: circulo-de-belleza-authentication
source_filename: circulo-de-belleza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.circulodebelleza.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  notes: >-\n    Storefront authentication is Shopify Customer Accounts (OIDC). Issuer is\n    Shopify (shop_id 25099010151). Buyer-facing sign-in only; there is no\n    first-party developer/API-key program for this merchant. Agent commerce is\n    authorized per-checkout with buyer approval, not a long-lived merchant token.\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.circulodebelleza.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/25099010151\n  authorizationUrl: https://shopify.com/authentication/25099010151/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/25099010151/oauth/token\n  jwks_uri: https://shopify.com/authentication/25099010151/.well-known/jwks.json\n\
  \  end_session_endpoint: https://shopify.com/authentication/25099010151/logout\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  sources: [well-known/circulo-de-belleza-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circulo-de-belleza/refs/heads/main/authentication/circulo-de-belleza-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Beauty
- Cosmetics
- E-Commerce
- Retail
- Mexico
- Hair Care
- Professional Beauty Products
- Shopify
- Agent Commerce
---
