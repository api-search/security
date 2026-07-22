---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Boldfit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boldfit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Boldfit
provider_slug: boldfit
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/9646211123/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/9646211123/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/9646211123
  jwks_uri: https://shopify.com/authentication/9646211123/.well-known/jwks.json
  name: shopify_customer_account
  protocol: OpenID Connect (OAuth 2.0 Authorization Code + PKCE)
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/9646211123/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
slug: boldfit-authentication
source_filename: boldfit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.boldfit.com/.well-known/openid-configuration\nnotes: >-\n  Boldfit runs on Shopify. Programmatic access is the Shopify Customer Account\n  API, protected by OAuth 2.0 / OpenID Connect. The shop's discovery document\n  (issuer https://shopify.com/authentication/9646211123) defines the endpoints\n  and scopes below. This is customer-scoped auth (a shopper authorizing an app\n  to act on their own account), not a partner/admin API key surface. There is\n  no first-party developer program or API key issuance published by Boldfit.\nschemes:\n- type: oauth2\n  name: shopify_customer_account\n  protocol: OpenID Connect (OAuth 2.0 Authorization Code + PKCE)\n  issuer: https://shopify.com/authentication/9646211123\n  authorization_endpoint: https://shopify.com/authentication/9646211123/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/9646211123/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/9646211123/logout\n\
  \  jwks_uri: https://shopify.com/authentication/9646211123/.well-known/jwks.json\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boldfit/refs/heads/main/authentication/boldfit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consumer
- Fitness
- Sportswear
- E-Commerce
- Retail
- Shopify
---
