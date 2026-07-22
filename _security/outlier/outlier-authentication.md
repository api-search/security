---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Outlier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Outlier secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Outlier
provider_slug: outlier
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/40681930915/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/40681930915/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/40681930915
  jwks_uri: https://shopify.com/authentication/40681930915/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.outlier.org/.well-known/openid-configuration
  response_types:
  - code
  sources:
  - well-known/outlier-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/40681930915/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: outlier-authentication
source_filename: outlier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.outlier.org/.well-known/openid-configuration\ndocs: https://www.outlier.org/agents.md\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  notes: >-\n    Customer authentication is delegated to the Shopify Customer Account API\n    (issuer https://shopify.com/authentication/40681930915). Read-only catalog\n    browsing (product/collection JSON) requires no authentication.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.outlier.org/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/40681930915\n  authorizationUrl: https://shopify.com/authentication/40681930915/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/40681930915/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/40681930915/logout\n  jwks_uri: https://shopify.com/authentication/40681930915/.well-known/jwks.json\n\
  \  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  sources:\n  - well-known/outlier-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outlier/refs/heads/main/authentication/outlier-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Education
- Online Learning
- Dual Enrollment
- E-Commerce
- Shopify
- Agent Commerce
- MCP
---
