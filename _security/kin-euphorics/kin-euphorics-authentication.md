---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kin Euphorics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kin Euphorics secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kin Euphorics
provider_slug: kin-euphorics
scheme_count: 1
schemes:
- authorization_endpoint: https://account.kineuphorics.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.kineuphorics.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/27087620
  jwks_uri: https://account.kineuphorics.com/authentication/.well-known/jwks.json
  name: shopifyCustomerAccountsOIDC
  openIdConnectUrl: https://www.kineuphorics.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/kin-euphorics-openid-configuration.json
  token_endpoint: https://account.kineuphorics.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: kin-euphorics-authentication
source_filename: kin-euphorics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.kineuphorics.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  provider: Shopify Customer Accounts\nschemes:\n- name: shopifyCustomerAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.kineuphorics.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/27087620\n  authorization_endpoint: https://account.kineuphorics.com/authentication/oauth/authorize\n  token_endpoint: https://account.kineuphorics.com/authentication/oauth/token\n  end_session_endpoint: https://account.kineuphorics.com/authentication/logout\n  jwks_uri: https://account.kineuphorics.com/authentication/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types:\n  - code\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  code_challenge_methods:\n  - S256\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/kin-euphorics-openid-configuration.json\nnotes: >-\n  Authentication is provided by Shopify Customer Accounts (OpenID Connect /\n  OAuth 2.0 authorization-code flow with PKCE S256). The customer-account\n  issuer also advertises a customer-account-mcp-api:full scope, enabling\n  authenticated MCP access to a shopper's account context.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kin-euphorics/refs/heads/main/authentication/kin-euphorics-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Beverages
- Non-Alcoholic
- Functional Beverage
- Adaptogens
- Nootropics
- Consumer Packaged Goods
- Ecommerce
- Shopify
- Direct to Consumer
- Agentic Commerce
- UCP
- MCP
---
