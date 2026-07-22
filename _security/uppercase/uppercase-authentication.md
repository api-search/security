---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: Authentication profile for the uppercase storefront's machine surfaces, captured from the OIDC discovery and OAuth authorization-server documents served on uppercase.co.in (Shopify customer accounts, issuer https://shopify.com/authentication/67539140858). Customer-facing API and MCP access uses OAuth 2.0 authorization-code with PKCE (S256) plus refresh tokens and JWT bearer grant; unauthenticated read-only browsing of product and collection JSON is documented in /llms.txt. There is no first-party developer key program — auth is the Shopify platform surface on the store's own domain.
kind: authentication
layout: security
method: searched
name: Uppercase Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Uppercase secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Uppercase
provider_slug: uppercase
scheme_count: 2
schemes:
- issuer: https://shopify.com/authentication/67539140858
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://uppercase.co.in/.well-known/openid-configuration
  sources:
  - well-known/uppercase-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/67539140858/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/67539140858/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  name: shopify-customer-accounts-oauth2
  sources:
  - well-known/uppercase-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
slug: uppercase-authentication
source_filename: uppercase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://uppercase.co.in/.well-known/openid-configuration\ndescription: >-\n  Authentication profile for the uppercase storefront's machine surfaces,\n  captured from the OIDC discovery and OAuth authorization-server documents\n  served on uppercase.co.in (Shopify customer accounts, issuer\n  https://shopify.com/authentication/67539140858). Customer-facing API and\n  MCP access uses OAuth 2.0 authorization-code with PKCE (S256) plus refresh\n  tokens and JWT bearer grant; unauthenticated read-only browsing of product\n  and collection JSON is documented in /llms.txt. There is no first-party\n  developer key program — auth is the Shopify platform surface on the store's\n  own domain.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  unauthenticated_read: true\nschemes:\n  - name: shopify-customer-accounts-oidc\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/67539140858\n\
  \    openIdConnectUrl: https://uppercase.co.in/.well-known/openid-configuration\n    sources: [well-known/uppercase-openid-configuration.json]\n  - name: shopify-customer-accounts-oauth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/67539140858/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/67539140858/oauth/token\n        pkce: S256\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    token_endpoint_auth_methods: [client_secret_basic]\n    sources: [well-known/uppercase-oauth-authorization-server.json]\nrelated:\n  - scopes/uppercase-scopes.yml\n  - well-known/uppercase-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uppercase/refs/heads/main/authentication/uppercase-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Travel
- Luggage
- Backpacks
- Ecommerce
- Retail
- Sustainability
- Agentic Commerce
---
