---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Miyokos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Miyokos declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Miyokos
provider_slug: miyokos
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/5819545/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/5819545/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/5819545
  jwks_uri: https://shopify.com/authentication/5819545/.well-known/jwks.json
  name: shopify-customer-account-oidc
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/5819545/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: miyokos-authentication
source_filename: miyokos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://miyokos.com/.well-known/openid-configuration and /.well-known/oauth-authorization-server\nsummary: >-\n  Authentication is Shopify Customer Accounts (OpenID Connect / OAuth 2.0).\n  There is no first-party developer API key program; the identity layer is\n  provided by Shopify for the storefront's customer accounts and for UCP\n  agent-commerce authorization.\nschemes:\n- type: openIdConnect\n  name: shopify-customer-account-oidc\n  issuer: https://shopify.com/authentication/5819545\n  authorization_endpoint: https://shopify.com/authentication/5819545/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/5819545/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/5819545/logout\n  jwks_uri: https://shopify.com/authentication/5819545/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n\
  \  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\npkce: required (S256)\nnotes: >-\n  Agent commerce (UCP MCP) is unauthenticated for browsing/discovery; checkout\n  requires contemporaneous buyer approval routed through Shop Pay rather than a\n  client credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miyokos/refs/heads/main/authentication/miyokos-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Planetary Health
- Plant-Based
- Food and Beverage
- E-Commerce
- Shopify
- Agent Commerce
- UCP
---
