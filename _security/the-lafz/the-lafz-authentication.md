---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: The Lafz Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Lafz declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The Lafz
provider_slug: the-lafz
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/75100487925/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/75100487925/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/75100487925
  jwks_uri: https://shopify.com/authentication/75100487925/.well-known/jwks.json
  name: shopify-customer-account
  openid_configuration: https://shopify.com/authentication/75100487925/.well-known/openid-configuration
  pkce: true
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/75100487925/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: the-lafz-authentication
source_filename: the-lafz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  Fetched live from lafz.com/.well-known/openid-configuration (Shopify\n  customer-account OpenID Connect discovery document).\nsummary: >-\n  Customer authentication is delegated to Shopify's customer-account OpenID\n  Connect / OAuth 2.0 provider. There is no first-party Lafz auth server; the\n  issuer is a Shopify authentication tenant.\nschemes:\n- type: openIdConnect\n  name: shopify-customer-account\n  issuer: https://shopify.com/authentication/75100487925\n  openid_configuration: https://shopify.com/authentication/75100487925/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/75100487925/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/75100487925/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/75100487925/logout\n  jwks_uri: https://shopify.com/authentication/75100487925/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n\
  \  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types_supported:\n  - code\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  pkce: true\nnotes: >-\n  The customer-account-mcp-api:full scope indicates Shopify's customer-account\n  MCP API is available for authenticated agent access, distinct from the\n  unauthenticated UCP shopping MCP endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-lafz/refs/heads/main/authentication/the-lafz-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consumer
- Cosmetics
- Personal Care
- E-Commerce
- Halal
- Shopify
- Agent Commerce
---
