---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Nara Organics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nara Organics secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nara Organics
provider_slug: nara-organics
scheme_count: 1
schemes:
- authorization_endpoint: https://account.nara.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.nara.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/74927341841
  jwks_uri: https://account.nara.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  response_types_supported:
  - code
  sources:
  - well-known/nara-organics-openid-configuration.json
  token_endpoint: https://account.nara.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: nara-organics-authentication
source_filename: nara-organics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nara.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  provider: Shopify Customer Account (OIDC)\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/74927341841\n  authorization_endpoint: https://account.nara.com/authentication/oauth/authorize\n  token_endpoint: https://account.nara.com/authentication/oauth/token\n  end_session_endpoint: https://account.nara.com/authentication/logout\n  jwks_uri: https://account.nara.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported:\
  \ [S256]\n  sources: [well-known/nara-organics-openid-configuration.json]\nnotes: >-\n  Authenticated customer-account access uses Shopify's OIDC provider. Read-only\n  storefront browsing (products, collections, search, product/collection JSON) needs\n  no authentication per /llms.txt. Agent commerce over the UCP MCP endpoint routes\n  payment approval through the buyer / Shop Pay rather than an agent-held credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nara-organics/refs/heads/main/authentication/nara-organics-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Commerce
- Retail
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Infant Formula
---
