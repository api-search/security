---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Piper Inc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Piper Inc. secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Piper Inc.
provider_slug: piper-inc
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/9256256/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/9256256/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/9256256
  jwks_uri: https://shopify.com/authentication/9256256/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.playpiper.in/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/9256256/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: piper-inc-authentication
source_filename: piper-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.playpiper.in/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Auth is Shopify Customer Account Authentication (OpenID Connect) for the Piper\n  store (id 9256256). Discovery published at /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server. Agent commerce (UCP MCP) additionally\n  uses the customer-account-mcp-api:full scope. No provider-authored OpenAPI is\n  published for this storefront.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/9256256\n  openIdConnectUrl: https://www.playpiper.in/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/9256256/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/9256256/oauth/token\n\
  \  end_session_endpoint: https://shopify.com/authentication/9256256/logout\n  jwks_uri: https://shopify.com/authentication/9256256/.well-known/jwks.json\n  response_types: [code]\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods: [client_secret_basic]\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piper-inc/refs/heads/main/authentication/piper-inc-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Education
- EdTech
- STEM
- Hardware
- E-Commerce
- Agentic Commerce
- MCP
- Shopify
---
