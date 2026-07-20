---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Candyclub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CandyClub secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CandyClub
provider_slug: candyclub
scheme_count: 1
schemes:
- authorization_endpoint: https://account.candyclub.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.candyclub.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/65295974459
  jwks_uri: https://account.candyclub.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://candyclub.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/candyclub-openid-configuration.json
  token_endpoint: https://account.candyclub.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: candyclub-authentication
source_filename: candyclub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://candyclub.com/.well-known/openid-configuration\ndocs: https://candyclub.com/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  notes: >-\n    Authentication is Shopify Customer Accounts (issuer\n    https://shopify.com/authentication/65295974459). Customer/agent access uses\n    OpenID Connect authorization-code flow with PKCE (S256). Agent commerce over\n    the UCP MCP endpoint additionally uses the customer-account-mcp-api scope.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://candyclub.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/65295974459\n    authorization_endpoint: https://account.candyclub.com/authentication/oauth/authorize\n    token_endpoint: https://account.candyclub.com/authentication/oauth/token\n    end_session_endpoint: https://account.candyclub.com/authentication/logout\n\
  \    jwks_uri: https://account.candyclub.com/authentication/.well-known/jwks.json\n    response_types_supported: [code]\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    code_challenge_methods_supported: [S256]\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    scopes_supported:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    sources: [well-known/candyclub-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candyclub/refs/heads/main/authentication/candyclub-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Candy
- Confectionery
- Ecommerce
- Subscription
- Retail
- Shopify
- Agent Commerce
- UCP
---
