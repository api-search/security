---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Barn And Willow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Barn & Willow secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Barn & Willow
provider_slug: barn-and-willow
scheme_count: 1
schemes:
- authorization_endpoint: https://account.barnandwillow.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.barnandwillow.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/4558913
  jwks_uri: https://account.barnandwillow.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://barnandwillow.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/barn-and-willow-openid-configuration.json
  token_endpoint: https://account.barnandwillow.com/authentication/oauth/token
  type: openIdConnect
slug: barn-and-willow-authentication
source_filename: barn-and-willow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://barnandwillow.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Barn & Willow runs on Shopify. Customer-facing authentication is the Shopify\n  Customer Account API, an OAuth 2.0 / OpenID Connect provider (issuer\n  https://shopify.com/authentication/4558913). Agentic commerce over the UCP MCP\n  endpoint uses the customer-account-mcp-api scope of the same provider.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth_methods: [client_secret_basic]\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://barnandwillow.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/4558913\n  authorization_endpoint: https://account.barnandwillow.com/authentication/oauth/authorize\n  token_endpoint: https://account.barnandwillow.com/authentication/oauth/token\n\
  \  end_session_endpoint: https://account.barnandwillow.com/authentication/logout\n  jwks_uri: https://account.barnandwillow.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  sources: [well-known/barn-and-willow-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barn-and-willow/refs/heads/main/authentication/barn-and-willow-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- E-commerce
- Retail
- Home Furnishings
- Window Treatments
- Agentic Commerce
- Shopify
- Direct to Consumer
---
