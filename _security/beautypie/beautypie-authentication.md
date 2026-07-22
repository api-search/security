---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Beautypie Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Beauty Pie secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Beauty Pie
provider_slug: beautypie
scheme_count: 2
schemes:
- issuer: https://shopify.com/authentication/73264758967
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.beautypie.com/.well-known/openid-configuration
  sources:
  - well-known/beautypie-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/73264758967/oauth/authorize
    endSessionUrl: https://shopify.com/authentication/73264758967/logout
    flow: authorizationCode
    pkce: S256
    scopes:
    - openid
    - email
    - customer-account-api:full
    - customer-account-mcp-api:full
    tokenUrl: https://shopify.com/authentication/73264758967/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  jwks_uri: https://shopify.com/authentication/73264758967/.well-known/jwks.json
  name: ShopifyCustomerAccountOAuth2
  response_types:
  - code
  sources:
  - well-known/beautypie-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
slug: beautypie-authentication
source_filename: beautypie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.beautypie.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Derived from the live OIDC/OAuth2 discovery document served under beautypie.com.\n  This is Shopify's Customer Account authentication (issuer\n  https://shopify.com/authentication/73264758967) fronting the beautypie.com store.\n  It governs authenticated customer-account access, not an open developer API.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  openid_connect: true\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.beautypie.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/73264758967\n  sources: [well-known/beautypie-openid-configuration.json]\n- name: ShopifyCustomerAccountOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/73264758967/oauth/authorize\n\
  \    tokenUrl: https://shopify.com/authentication/73264758967/oauth/token\n    endSessionUrl: https://shopify.com/authentication/73264758967/logout\n    pkce: S256\n    scopes: [openid, email, customer-account-api:full, customer-account-mcp-api:full]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  jwks_uri: https://shopify.com/authentication/73264758967/.well-known/jwks.json\n  sources: [well-known/beautypie-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beautypie/refs/heads/main/authentication/beautypie-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Beauty
- Skincare
- Cosmetics
- Ecommerce
- Direct-to-Consumer
- Membership
- Retail
- Shopify
- Storefront MCP
---
