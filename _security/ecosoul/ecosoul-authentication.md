---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ecosoul Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: EcoSoul Home secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: EcoSoul Home
provider_slug: ecosoul
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/49573396633/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/49573396633/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/49573396633
  jwks_uri: https://shopify.com/authentication/49573396633/.well-known/jwks.json
  name: ShopifyCustomerAccountsOIDC
  openIdConnectUrl: https://www.ecosoulhome.com/.well-known/openid-configuration
  response_types_supported:
  - code
  token_endpoint: https://shopify.com/authentication/49573396633/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: ecosoul-authentication
source_filename: ecosoul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.ecosoulhome.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Customer-facing authentication is Shopify Customer Accounts (OpenID Connect /\n  OAuth 2.0 authorization_code + PKCE). The OIDC issuer is Shopify, scoped to this\n  merchant (49573396633). Storefront read endpoints (product/collection JSON) require\n  no authentication; the agent-commerce UCP MCP endpoint additionally requires a UCP\n  agent profile and buyer approval at payment.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/49573396633\n  openIdConnectUrl: https://www.ecosoulhome.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/49573396633/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/49573396633/oauth/token\n\
  \  end_session_endpoint: https://shopify.com/authentication/49573396633/logout\n  jwks_uri: https://shopify.com/authentication/49573396633/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecosoul/refs/heads/main/authentication/ecosoul-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Sustainability
- Home Goods
- Compostable
- Tableware
- Retail
- E-Commerce
- Shopify
- Agentic Commerce
---
