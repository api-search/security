---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Everlane Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: everlane secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: everlane
provider_slug: everlane
scheme_count: 1
schemes:
- authorization_endpoint: https://account.everlane.com/authentication/oauth/authorize
  end_session_endpoint: https://account.everlane.com/authentication/logout
  issuer: https://shopify.com/authentication/62379163734
  jwks_uri: https://account.everlane.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://everlane.com/.well-known/openid-configuration
  response_types:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/everlane-openid-configuration.json
  token_endpoint: https://account.everlane.com/authentication/oauth/token
  type: openIdConnect
slug: everlane-authentication
source_filename: everlane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://everlane.com/.well-known/openid-configuration\ndocs: https://everlane.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: [S256]\n  token_endpoint_auth: [client_secret_basic]\n  id_token_signing: [RS256]\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/62379163734\n  openIdConnectUrl: https://everlane.com/.well-known/openid-configuration\n  authorization_endpoint: https://account.everlane.com/authentication/oauth/authorize\n  token_endpoint: https://account.everlane.com/authentication/oauth/token\n  jwks_uri: https://account.everlane.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.everlane.com/authentication/logout\n  response_types: [code]\n  scopes_supported:\
  \ [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: ['well-known/everlane-openid-configuration.json']\nnotes: Shopify-managed Customer Account authentication (OIDC/OAuth2) exposed on the account.everlane.com subdomain. The public storefront MCP at everlane.com/api/mcp is unauthenticated for read/cart; checkout requires buyer approval.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlane/refs/heads/main/authentication/everlane-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Fashion
- Direct-to-Consumer
- Shopify
- Agentic Commerce
---
