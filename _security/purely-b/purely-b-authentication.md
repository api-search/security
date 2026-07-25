---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Purely B Authentication
name_suffix: Authentication
oauth_flows: []
overview: Purely B declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Purely B
provider_slug: purely-b
scheme_count: 1
schemes:
- authorization_endpoint: https://account.purelyb.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.purelyb.com/authentication/logout
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_account_oauth
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/4610130033
  jwks_uri: https://account.purelyb.com/authentication/.well-known/jwks.json
  pkce: true
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://account.purelyb.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: purely-b-authentication
source_filename: purely-b-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://purelyb.com/.well-known/openid-configuration\nsummary: >-\n  PurelyB customer authentication is Shopify's Customer Account API OAuth 2.0 /\n  OpenID Connect provider. Storefront product browsing is unauthenticated; the\n  customer account + customer-account MCP surfaces are OAuth-protected.\nschemes:\n- id: shopify_customer_account_oauth\n  type: openIdConnect\n  flow: authorization_code\n  pkce: true\n  code_challenge_methods:\n  - S256\n  issuer: https://shopify.com/authentication/4610130033\n  authorization_endpoint: https://account.purelyb.com/authentication/oauth/authorize\n  token_endpoint: https://account.purelyb.com/authentication/oauth/token\n  end_session_endpoint: https://account.purelyb.com/authentication/logout\n  jwks_uri: https://account.purelyb.com/authentication/.well-known/jwks.json\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  grant_types_supported:\n  - authorization_code\n\
  \  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  id_token_signing_alg: RS256\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  response_types_supported:\n  - code\npublic_surfaces:\n- description: Read-only storefront browsing requires no authentication (products.json, collections, search).\n  source: https://purelyb.com/llms.txt\nnotes:\n- Standards-conformant OIDC (discovery, PKCE S256, RS256 id_token) provisioned by Shopify.\n- op_policy_uri and op_tos_uri point to Shopify legal, confirming platform-managed identity.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purely-b/refs/heads/main/authentication/purely-b-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Wellness
- E-Commerce
- Supplements
- Shopify
- Agentic Commerce
- MCP
---
