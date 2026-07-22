---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Because Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Because secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Because
provider_slug: because
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/61841768621/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/61841768621/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/61841768621
  jwks_uri: https://shopify.com/authentication/61841768621/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://becausemarket.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/because-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/61841768621/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: because-authentication
source_filename: because-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://becausemarket.com/.well-known/openid-configuration\ndocs: https://becausemarket.com/account/login\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    Customer-facing authentication is Shopify Customer Accounts (OIDC), surfaced on\n    the storefront domain via /.well-known/openid-configuration. The storefront has\n    no separately published first-party developer API; agent commerce authenticates\n    through the UCP shopping service (buyer approval at payment), not a bearer API key.\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://becausemarket.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/61841768621\n  authorization_endpoint: https://shopify.com/authentication/61841768621/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/61841768621/oauth/token\n  end_session_endpoint:\
  \ https://shopify.com/authentication/61841768621/logout\n  jwks_uri: https://shopify.com/authentication/61841768621/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - S256\n  sources:\n  - well-known/because-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/because/refs/heads/main/authentication/because-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Retail
- E-commerce
- Health
- Incontinence
- Senior Care
- Agentic Commerce
- Shopify
---
