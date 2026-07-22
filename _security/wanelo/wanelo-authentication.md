---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Wanelo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: wanelo secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: wanelo
provider_slug: wanelo
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/69560926386/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/69560926386/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/69560926386
  jwks_uri: https://shopify.com/authentication/69560926386/.well-known/jwks.json
  name: shopifyCustomerAccount
  openIdConnectUrl: https://wanelo.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/wanelo-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/69560926386/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: wanelo-authentication
source_filename: wanelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://wanelo.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  provider: Shopify Customer Accounts\n  note: >-\n    wanelo.com is a Shopify storefront; buyer/customer authentication is delegated\n    to Shopify's Customer Account identity provider (issuer\n    https://shopify.com/authentication/69560926386). Read-only catalog browsing\n    (products/collections/search JSON) requires no authentication.\nschemes:\n  - name: shopifyCustomerAccount\n    type: openIdConnect\n    openIdConnectUrl: https://wanelo.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/69560926386\n    authorization_endpoint: https://shopify.com/authentication/69560926386/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/69560926386/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/69560926386/logout\n\
  \    jwks_uri: https://shopify.com/authentication/69560926386/.well-known/jwks.json\n    response_types_supported: [code]\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    id_token_signing_alg_values_supported: [RS256]\n    sources: [well-known/wanelo-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wanelo/refs/heads/main/authentication/wanelo-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Shopping
- Ecommerce
- Retail
- Commerce
- Agent Commerce
- MCP
- Shopify
- AI
---
