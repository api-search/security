---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: True And Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: True & Co declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: True & Co
provider_slug: true-and-co
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/86218834196/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/86218834196/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/86218834196
  jwks_uri: https://shopify.com/authentication/86218834196/.well-known/jwks.json
  name: shopify-customer-account
  openid_configuration: https://trueandco.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/86218834196/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: true-and-co-authentication
source_filename: true-and-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: 2026-07-21\nmethod: searched\nsource: >-\n  https://trueandco.com/.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server, fetched live 2026-07-21\nsummary: >-\n  Buyer authentication is handled by Shopify Customer Accounts using OAuth 2.0 /\n  OpenID Connect. The store domain publishes live OIDC and OAuth Authorization\n  Server metadata. Agent commerce over the UCP/MCP endpoint layers on top of this\n  identity, and payment completion always requires human buyer approval.\nschemes:\n- type: openIdConnect\n  name: shopify-customer-account\n  issuer: https://shopify.com/authentication/86218834196\n  openid_configuration: https://trueandco.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/86218834196/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/86218834196/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/86218834196/logout\n  jwks_uri: https://shopify.com/authentication/86218834196/.well-known/jwks.json\n\
  \  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-and-co/refs/heads/main/authentication/true-and-co-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Apparel
- Intimates
- Agentic Commerce
- Shopify
- MCP
---
