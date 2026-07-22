---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Earable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Earable secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Earable
provider_slug: earable
scheme_count: 1
schemes:
- authorization_endpoint: https://account.frenzband.com/authentication/oauth/authorize
  end_session_endpoint: https://account.frenzband.com/authentication/logout
  issuer: https://shopify.com/authentication/66693300444
  jwks_uri: https://account.frenzband.com/authentication/.well-known/jwks.json
  name: shopify-customer-account
  openIdConnectUrl: https://frenzband.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://account.frenzband.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: earable-authentication
source_filename: earable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://frenzband.com/.well-known/openid-configuration\nnotes: >-\n  Auth on the frenzband.com storefront is the Shopify Customer Account API\n  (OIDC/OAuth2), advertised at /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server. Platform-provided by Shopify; there is\n  no first-party Earable developer API. Endpoints resolve under\n  account.frenzband.com.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: shopify-customer-account\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/66693300444\n  openIdConnectUrl: https://frenzband.com/.well-known/openid-configuration\n  authorization_endpoint: https://account.frenzband.com/authentication/oauth/authorize\n  token_endpoint: https://account.frenzband.com/authentication/oauth/token\n  end_session_endpoint: https://account.frenzband.com/authentication/logout\n  jwks_uri: https://account.frenzband.com/authentication/.well-known/jwks.json\n\
  \  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earable/refs/heads/main/authentication/earable-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Wearables
- Sleep Technology
- Neuroscience
- Health
- Consumer Electronics
- Agentic Commerce
- Shopify
---
