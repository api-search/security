---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Aventon Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Aventon secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Aventon
provider_slug: aventon
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/15202468/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/15202468/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/15202468
  jwks_uri: https://shopify.com/authentication/15202468/.well-known/jwks.json
  name: shopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.aventon.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/aventon-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/15202468/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: aventon-authentication
source_filename: aventon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.aventon.com/.well-known/openid-configuration\ndocs: https://www.aventon.com/.well-known/oauth-authorization-server\nnotes: >-\n  Authentication surface is Shopify's Customer Account API OpenID Connect, exposed\n  on the aventon.com domain. Authorization Code flow with PKCE (S256). The\n  customer-account-mcp-api:full scope gates the agent/MCP commerce surface.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  issuer: https://shopify.com/authentication/15202468\nschemes:\n- name: shopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.aventon.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/15202468\n  authorization_endpoint: https://shopify.com/authentication/15202468/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/15202468/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/15202468/logout\n\
  \  jwks_uri: https://shopify.com/authentication/15202468/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  sources: [well-known/aventon-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aventon/refs/heads/main/authentication/aventon-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Electric Bikes
- E-Commerce
- Retail
- Agent Commerce
- Shopify
- Universal Commerce Protocol
---
