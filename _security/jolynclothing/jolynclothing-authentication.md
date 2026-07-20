---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jolynclothing Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: JOLYN secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: JOLYN
provider_slug: jolynclothing
scheme_count: 1
schemes:
- authorization_endpoint: https://account.jolyn.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.jolyn.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/7030099
  jwks_uri: https://account.jolyn.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccount
  openIdConnectUrl: https://jolyn.com/.well-known/openid-configuration
  response_types:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/jolynclothing-openid-configuration.json
  token_endpoint: https://account.jolyn.com/authentication/oauth/token
  type: openIdConnect
slug: jolynclothing-authentication
source_filename: jolynclothing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://jolyn.com/.well-known/openid-configuration\nnote: >-\n  JOLYN publishes no first-party developer API. Its storefront (jolyn.com) is Shopify-hosted\n  and exposes the Shopify Customer Account API OIDC discovery document plus a UCP agent MCP\n  endpoint. The auth profile below is captured verbatim from the live OIDC discovery document.\n  Read-only storefront browsing (/products/{handle}.json, /collections/{handle}/products.json)\n  requires no authentication.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth: client_secret_basic\nschemes:\n  - name: ShopifyCustomerAccount\n    type: openIdConnect\n    openIdConnectUrl: https://jolyn.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/7030099\n    authorization_endpoint: https://account.jolyn.com/authentication/oauth/authorize\n    token_endpoint: https://account.jolyn.com/authentication/oauth/token\n\
  \    end_session_endpoint: https://account.jolyn.com/authentication/logout\n    jwks_uri: https://account.jolyn.com/authentication/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:jwt-bearer\"]\n    response_types: [code]\n    id_token_signing_alg: [RS256]\n    code_challenge_methods: [S256]\n    scopes_supported: [openid, email, \"customer-account-api:full\", \"customer-account-mcp-api:full\"]\n    sources: [well-known/jolynclothing-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jolynclothing/refs/heads/main/authentication/jolynclothing-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Swimwear
- Direct-to-Consumer
- Shopify
- Agentic Commerce
---
