---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: The Folklore Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: The Folklore secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: The Folklore
provider_slug: the-folklore
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/63533449453/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/63533449453/logout
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/63533449453
  jwks_uri: https://shopify.com/authentication/63533449453/.well-known/jwks.json
  name: shopifyCustomerAccountOIDC
  openIdConnectUrl: https://thefolklore.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/63533449453/oauth/token
  type: openIdConnect
slug: the-folklore-authentication
source_filename: the-folklore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://thefolklore.com/.well-known/openid-configuration\nnote: >-\n  Authentication is provided by the Shopify Customer Account API via OpenID\n  Connect / OAuth 2.0. Values transcribed verbatim from the store's live OIDC\n  discovery document. There is no first-party OpenAPI to derive from; the\n  customer-account-mcp-api:full scope gates the UCP MCP commerce surface.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: S256\n  token_endpoint_auth: client_secret_basic\nschemes:\n- name: shopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/63533449453\n  openIdConnectUrl: https://thefolklore.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/63533449453/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/63533449453/oauth/token\n\
  \  end_session_endpoint: https://shopify.com/authentication/63533449453/logout\n  jwks_uri: https://shopify.com/authentication/63533449453/.well-known/jwks.json\n  id_token_signing_alg: RS256\n  code_challenge_methods: [S256]\n  response_types: [code]\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-folklore/refs/heads/main/authentication/the-folklore-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Commerce
- Wholesale
- Marketplace
- Retail
- E-commerce
- Fashion
- Agentic Commerce
- Shopify
---
