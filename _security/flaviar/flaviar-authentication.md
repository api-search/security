---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Flaviar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Flaviar secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Flaviar
provider_slug: flaviar
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/80863265050/oauth/authorize
  endSessionUrl: https://shopify.com/authentication/80863265050/logout
  issuer: https://shopify.com/authentication/80863265050
  jwksUri: https://shopify.com/authentication/80863265050/.well-known/jwks.json
  name: ShopifyCustomerAccount
  openIdConnectUrl: https://flaviar.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/flaviar-openid-configuration.json
  - well-known/flaviar-oauth-authorization-server.json
  tokenUrl: https://shopify.com/authentication/80863265050/oauth/token
  type: openIdConnect
slug: flaviar-authentication
source_filename: flaviar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://flaviar.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Customer-facing authentication on the Flaviar storefront is delegated to\n  Shopify's Customer Account authorization server (OAuth 2.0 + OpenID Connect,\n  issuer https://shopify.com/authentication/80863265050). Derived from the live\n  OIDC discovery and RFC 8414 authorization-server metadata documents.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth: [client_secret_basic]\n  id_token_signing: [RS256]\nschemes:\n  - name: ShopifyCustomerAccount\n    type: openIdConnect\n    openIdConnectUrl: https://flaviar.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/80863265050\n    authorizationUrl: https://shopify.com/authentication/80863265050/oauth/authorize\n\
  \    tokenUrl: https://shopify.com/authentication/80863265050/oauth/token\n    endSessionUrl: https://shopify.com/authentication/80863265050/logout\n    jwksUri: https://shopify.com/authentication/80863265050/.well-known/jwks.json\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    sources: [well-known/flaviar-openid-configuration.json, well-known/flaviar-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flaviar/refs/heads/main/authentication/flaviar-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Spirits
- Whiskey
- Ecommerce
- Retail
- Beverages
- Subscription
- Agent Commerce
- Shopify
---
