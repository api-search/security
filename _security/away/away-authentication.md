---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Away Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Away secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Away
provider_slug: away
scheme_count: 1
schemes:
- authorization_endpoint: https://accounts.awaytravel.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://accounts.awaytravel.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/66474180792
  jwks_uri: https://accounts.awaytravel.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccounts
  openIdConnectUrl: https://www.awaytravel.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/away-openid-configuration.json
  token_endpoint: https://accounts.awaytravel.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: away-authentication
source_filename: away-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.awaytravel.com/.well-known/openid-configuration\ndocs: https://www.awaytravel.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  note: >-\n    Away runs on Shopify; customer-facing auth is Shopify Customer Accounts\n    (OpenID Connect). The storefront browse/catalog surface is unauthenticated;\n    checkout is buyer-authorized. No first-party developer API-key program.\nschemes:\n- name: ShopifyCustomerAccounts\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/66474180792\n  openIdConnectUrl: https://www.awaytravel.com/.well-known/openid-configuration\n  authorization_endpoint: https://accounts.awaytravel.com/authentication/oauth/authorize\n  token_endpoint: https://accounts.awaytravel.com/authentication/oauth/token\n  end_session_endpoint: https://accounts.awaytravel.com/authentication/logout\n  jwks_uri:\
  \ https://accounts.awaytravel.com/authentication/.well-known/jwks.json\n  response_types: [code]\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/away-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/away/refs/heads/main/authentication/away-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Travel
- Retail
- E-commerce
- Luggage
- Agent Commerce
- Shopify
- MCP
---
