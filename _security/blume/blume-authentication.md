---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Blume Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Blume secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Blume
provider_slug: blume
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/345800755/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/345800755/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/345800755
  jwks_uri: https://shopify.com/authentication/345800755/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.blume.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/blume-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/345800755/oauth/token
  type: openIdConnect
slug: blume-authentication
source_filename: blume-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.blume.com/.well-known/openid-configuration\nnotes: >-\n  Authentication for the blume.com storefront is provided by the Shopify Customer\n  Account API (OAuth2 authorization_code with PKCE + OpenID Connect). Discovered\n  live from the store's OIDC discovery document. This is the buyer/customer auth\n  surface; agent commerce over the UCP MCP endpoint additionally requires a UCP\n  agent profile handshake.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth: client_secret_basic\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/345800755\n    openIdConnectUrl: https://www.blume.com/.well-known/openid-configuration\n    authorization_endpoint: https://shopify.com/authentication/345800755/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/345800755/oauth/token\n\
  \    end_session_endpoint: https://shopify.com/authentication/345800755/logout\n    jwks_uri: https://shopify.com/authentication/345800755/.well-known/jwks.json\n    id_token_signing_alg: [RS256]\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    code_challenge_methods: [S256]\n    scopes:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    sources: [well-known/blume-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blume/refs/heads/main/authentication/blume-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Skincare
- Beauty
- Self-Care
- E-commerce
- Consumer
- Shopify
- Agent Commerce
- Universal Commerce Protocol
- MCP
---
