---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Source Beauty Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Source Beauty secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Source Beauty
provider_slug: source-beauty
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/68449239327/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/68449239327/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/68449239327
  jwks_uri: https://shopify.com/authentication/68449239327/.well-known/jwks.json
  name: ShopifyCustomerAccount
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/68449239327/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: source-beauty-authentication
source_filename: source-beauty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://sourcebeauty.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  notes: >-\n    Storefront customer authentication is delegated to the Shopify Customer Account\n    authorization server (issuer https://shopify.com/authentication/68449239327),\n    discoverable at /.well-known/openid-configuration and /.well-known/oauth-authorization-server.\n    This is the customer/agent identity layer; the store itself publishes no separate\n    first-party developer API.\nschemes:\n- name: ShopifyCustomerAccount\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/68449239327\n  authorization_endpoint: https://shopify.com/authentication/68449239327/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/68449239327/oauth/token\n  jwks_uri: https://shopify.com/authentication/68449239327/.well-known/jwks.json\n\
  \  end_session_endpoint: https://shopify.com/authentication/68449239327/logout\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [S256]\n  scopes_supported: [openid, email, customer-account-api:full, customer-account-mcp-api:full]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/source-beauty/refs/heads/main/authentication/source-beauty-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Beauty
- Cosmetics
- E-commerce
- Retail
- Marketplace
- Wellness
- Egypt
- Skincare
- Consumer
---
