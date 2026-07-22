---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Baublebar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BaubleBar secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BaubleBar
provider_slug: baublebar
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/26757464148/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/26757464148/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/26757464148
  jwks_uri: https://shopify.com/authentication/26757464148/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/baublebar-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/26757464148/oauth/token
  type: openIdConnect
slug: baublebar-authentication
source_filename: baublebar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.baublebar.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  BaubleBar authenticates customers through Shopify's Customer Account API\n  (OpenID Connect / OAuth 2.0). Values below are transcribed verbatim from the\n  shop's live OIDC discovery document (issuer https://shopify.com/authentication/26757464148).\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth_methods: [client_secret_basic]\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/26757464148\n    authorization_endpoint: https://shopify.com/authentication/26757464148/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/26757464148/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/26757464148/logout\n    jwks_uri: https://shopify.com/authentication/26757464148/.well-known/jwks.json\n\
  \    response_types_supported: [code]\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    id_token_signing_alg_values_supported: [RS256]\n    code_challenge_methods_supported: [S256]\n    scopes_supported:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    sources: [well-known/baublebar-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baublebar/refs/heads/main/authentication/baublebar-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Retail
- E-commerce
- Jewelry
- Accessories
- Fashion
- Shopify
- MCP
---
