---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cotopaxi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cotopaxi secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cotopaxi
provider_slug: cotopaxi
scheme_count: 2
schemes:
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/2817544
  name: ShopifyCustomerAccountsOIDC
  openIdConnectUrl: https://www.cotopaxi.com/.well-known/openid-configuration
  sources:
  - well-known/cotopaxi-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://account.cotopaxi.com/authentication/oauth/authorize
    end_session_endpoint: https://account.cotopaxi.com/authentication/logout
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    - urn:ietf:params:oauth:grant-type:jwt-bearer
    scopes:
    - openid
    - email
    - customer-account-api:full
    - customer-account-mcp-api:full
    tokenUrl: https://account.cotopaxi.com/authentication/oauth/token
  name: ShopifyCustomerAccountsOAuth2
  sources:
  - well-known/cotopaxi-oauth-authorization-server.json
  type: oauth2
slug: cotopaxi-authentication
source_filename: cotopaxi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cotopaxi.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Derived from the live OIDC/OAuth authorization-server discovery documents for\n  the Cotopaxi Shopify shop. This is Shopify Customer Accounts OAuth2/OIDC; there\n  is no first-party Cotopaxi developer API. Endpoints are served from\n  account.cotopaxi.com under the shared Shopify issuer.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  pkce_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.cotopaxi.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/2817544\n  id_token_signing_alg: [RS256]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources: [well-known/cotopaxi-openid-configuration.json]\n\
  - name: ShopifyCustomerAccountsOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.cotopaxi.com/authentication/oauth/authorize\n    tokenUrl: https://account.cotopaxi.com/authentication/oauth/token\n    end_session_endpoint: https://account.cotopaxi.com/authentication/logout\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/cotopaxi-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cotopaxi/refs/heads/main/authentication/cotopaxi-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Outdoor
- Apparel
- Ecommerce
- Retail
- Shopify
- MCP
---
