---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: Buyer identity on the Molekule storefront is handled by the Shopify Customer Account API, which publishes an OpenID Connect discovery document at /.well-known/openid-configuration. The issuer is the Shopify authentication service for this store (shopify.com/authentication/70884294938).
kind: authentication
layout: security
method: searched
name: Molekule Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Molekule secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Molekule
provider_slug: molekule
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/70884294938/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/70884294938/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/70884294938
  jwks_uri: https://shopify.com/authentication/70884294938/.well-known/jwks.json
  name: shopifyCustomerAccountOIDC
  openIdConnectUrl: https://molekule.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/molekule-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/70884294938/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: molekule-authentication
source_filename: molekule-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://molekule.com/.well-known/openid-configuration\ndescription: >-\n  Buyer identity on the Molekule storefront is handled by the Shopify Customer\n  Account API, which publishes an OpenID Connect discovery document at\n  /.well-known/openid-configuration. The issuer is the Shopify authentication\n  service for this store (shopify.com/authentication/70884294938).\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\nschemes:\n- name: shopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://molekule.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/70884294938\n  authorization_endpoint: https://shopify.com/authentication/70884294938/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/70884294938/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/70884294938/logout\n  jwks_uri:\
  \ https://shopify.com/authentication/70884294938/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  sources:\n  - well-known/molekule-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/molekule/refs/heads/main/authentication/molekule-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Hardware
- Air Quality
- Consumer IoT
- E-Commerce
- Agent Commerce
- MCP
- Shopify
---
