---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ami Paris Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AMI Paris secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AMI Paris
provider_slug: ami-paris
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/77478658352/oauth/authorize
  code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/77478658352
  jwks_uri: https://shopify.com/authentication/77478658352/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openid_configuration: well-known/ami-paris-openid-configuration.json
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/77478658352/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: ami-paris-authentication
source_filename: ami-paris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.amiparis.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  AMI Paris runs on Shopify. Storefront product/collection browsing is\n  unauthenticated (public JSON endpoints). Authenticated customer access uses the\n  Shopify Customer Account OIDC/OAuth2 authorization server (issuer scoped to this\n  store's merchant id 77478658352). The UCP agent-commerce MCP endpoint additionally\n  requires an agent-profile handshake.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/77478658352\n  openid_configuration: well-known/ami-paris-openid-configuration.json\n  authorization_endpoint: https://shopify.com/authentication/77478658352/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/77478658352/oauth/token\n\
  \  jwks_uri: https://shopify.com/authentication/77478658352/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ami-paris/refs/heads/main/authentication/ami-paris-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Fashion
- Retail
- Ecommerce
- Shopify
- Agent Commerce
- UCP
---
